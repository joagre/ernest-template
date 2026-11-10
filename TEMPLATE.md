# The template's design

What `ernest-template` is, and why each of its files is there. This is the template's own document and not a copy's: the last step of `README.md` removes it. It states the design as it stands, and changes with the template. The template's history, where each rule came from and what each application taught it, is `TEMPLATE_LOG.md`'s.

## 1. What it is for

An application written in Ernest is not the language. It has no report of its own, no compiler, no Erlang of its own, no readers of a language, and no section numbers for tests to cite. What it shares with Ernest's repository is the way of working: a plan that says what is built and when, a log that says why, a proposal discussed until it is solid, a test before every commit, a read-back before a report, a stop after each item, and the owner of each fact decided before a sentence is written.

The template holds that way of working in a form small enough that a new application starts from it in one copy and one edit. It is a template and not a framework: it holds no code of its own but a launcher and one checker, and it decides nothing about the program's design. A library starts from the same template, with no `main` and no launcher.

The applications are where the language is used in anger. Each keeps `language_feedback.md` under `docs/` in the shape of Ernest's file of that name, a queue: a line is carried there by Ernest's issue tracker, or, for an application built in Ernest's clean room, by a message to its session, and then goes, and the file goes when it is empty, Ernest's file being the record; that road back is the template's reason to exist.

## 2. What an application needs of the toolchain

Everything the template does, the toolchain does already; the template only chooses the roots and names them once.

- `ern build --source-root src --build-root build src` compiles every module under `src/`, mirroring the tree into `build/`, in dependency order, and does nothing for a module whose source and dependencies have not changed (report §11.1). Without `--build-root` a module compiles beside its source, so the Makefile always names the two roots.
- A module's namespace is its path under the source root (§4.2). Each directory between a load-path root and a module is lowercase words joined by `_`; the root's own name is not checked (§11.1, §11.2).
- A test is a top-level `let` of type `Test.Case(m)` in the module it tests (Appendix E.24), and `ern test build` runs the tests of every module under the build root (§11.2), so unit tests live in their modules.
- `ern format --check` names each module not in the layout (§11.6); `ern doc` writes a module's documentation (§11.4).
- `--load-path dir` is a root under which modules are found by namespace (§11.2), and `--libs-dir dir`, of `ern run`, `ern test` and `ern shell`, puts the `ebin` of each application under `dir` on the load path, so an Erlang module a `foreign fn` names is found there as a `.beam`, and a NIF's library from `priv/` beside `ebin/` (§8.4, §11.2). There is no package manager and no lockfile: a dependency is a directory.
- A compiled module is tied to the `ern` that built it, and one compiled against another interface or another standard library is refused before anything runs (§11.1, §11.2); two patch levels stand on one floor (§8.7).
- A program becomes a node by being started with `--config-dir dir` (§8.3, §11.3), whose `.ernest/` holds a private key. The operator's side is the deployment guide's, and the template restates none of it.
- Until 1.0 a release of `ern` may refuse a program the previous release accepted, so an application is written for one floor of `ern`.

## 3. The tree

A file is in the template only where it has content on the first day. `README.md`, `CLAUDE.md`, `LICENSE`, the Zero-Clause BSD license as Ernest's own, which the README names, `CHANGES.md`, `VERSION`, `Makefile`, `SECURITY.md` and `.gitignore` at the top; `bin/name`, the launcher, renamed for the program on the copy.

`README.md` says what the program is for its reader, then where to begin, with central links only and no argument the program's own documents make. `docs/README.md` says what each document is. `SECURITY.md` says where a security hole goes, and GitHub shows it in the repository's *Security* tab; the setting that takes such a report is not copied with the template, so a copy turns it on.

`.github/ISSUE_TEMPLATE/` holds a defect's issue form and a `config.yml`. The `config.yml` turns blank issues off and sends a security hole to private reporting. A copy changes the repository's address in it.

`assets/` holds the repository's icon, 128 by 128, and its social preview on GitHub, 1280 by 640, with a README saying what each is. GitHub takes the preview from the repository's settings, so a copy replaces both pictures with its own and uploads its preview there.

`src/name.ern` is the entry module, a placeholder the copy renames and writes, so that the template's own `make test` is green and a copy begins green. Its one test's comment cites every section of the starter design until real tests do. `tools/docs.ern` is the checker, a source root of its own built into `tools/build/` and outside the archive.

Under `docs/` stand `README.md`, `plan.md`, `log.md`, `design.md`, `release.md` and `full_review.md`. The rules an Ernest program is written by are not among them: they are Ernest's `guide/style.md`, installed beside `ern`, which `CLAUDE.md` names and a session reads from the installation.

What appears when needed, named in `CLAUDE.md` so that nothing waits for a decision about where it goes: `language_feedback.md` at its first line and `findings.md` while a review's findings are open, both under `docs/`; `docs/proposals/` with the first proposal; `test/`, a second source root for a program run end to end, built into `test/build/`; `erl/`, one read-only git submodule per Erlang application the program stands on, pinned and never a copy.

Also when needed: `THIRD_PARTY_LICENSES` with the first borrowed file, an Erlang application under `erl/` among them, since the archive carries its compiled code, and `ACKNOWLEDGMENTS.md` with the first name; for a library, `examples/`, a source root built into `examples/build/` whose every program `make examples` runs with one argument, `build/examples/<name>` and the Makefile's `EXAMPLE_SUFFIX`, and `make test` before its check of the documents; a program of `examples/` is an `.ern` file at its top, and what else stands under it is data.

Not committed: `build/`, each root's `build/`, `lib/` and `.ernest/`.

## 4. The Makefile, the launcher and the archive

One Makefile at the top. The variables an application edits stand first, and the rest is the same in every application, the same eleven targets among it: `all`, `test`, `examples`, `format`, `doc`, `run`, `lib`, `release`, `install`, `uninstall` and `clean`. There is no light run and no full run, since an application's whole suite runs in seconds, and where one day it does not, that is a defect of the tests to measure.

**The load path.** The libraries of Ernest's own stand on every job's load path by the toolchain's own rule (§11.1, §11.2). Everything else a program loads beyond the standard library stands under `lib/`, which `make lib` fills: `lib/<name>/build` for a dependency, a release archive fetched by its URL and unpacked once; `lib/<app>/ebin` for an Erlang application built by its own `make` under `erl/`, its `priv` linked beside it. The load path is `lib/*/build` for a dependency's modules and `--libs-dir lib` for the Erlang applications, in the Makefile and the launcher both, and no path is written twice.

`DEPS` and `ERL_DEPS` are in build order, a dependency before what needs it; the template resolves nothing, which is Ernest's decision for another day.

**The build.** `all` checks the floor, fills `lib/`, builds each dependency's `src/` into its own `build/` with the consumer's own `ern`, and then the program's `src/`.

**The floor.** `version` compares the first two numbers of `ern --version` with `ERN_VERSION` and refuses another floor with both texts; a development build of the floor, whose version text has `-dev` or `+<commit>` after the version (report §11.7), passes, since the applications are written against Ernest's unreleased builds to drive the language. `release` refuses a development build, in either form.

**The launcher.** `bin/<name>` runs `ern run` on the module its own name names, with each `lib/*/build` and `--libs-dir lib` of its root on the load path. Its root is `../lib/<name>/` where the module's compiled form stands there, beside an installed launcher, and `..` otherwise, a checkout or an unpacked archive: one file for the three. It forwards a leading `--config-dir dir`, the one option an operator gives, and everything after it to the program; the working directory stays the caller's.

**The archive.** `release` runs `test`, then writes `build/<name>-<version>.tar.gz`: the launcher where there is one, `src/`, `build/`, `lib/` with each link copied through, the user's documents, and the `Makefile` with `VERSION`, so that `make install` and `make run` run in the unpacked archive. One shape for an application and a library, so that any archive can be a dependency.

An archive carries the user's documents alone, each where it exists: `README.md`, `LICENSE`, `THIRD_PARTY_LICENSES`, `CHANGES.md`, `docs/design.md`, `examples/`, `deploy/` and `assets/`, whose pictures the documents show, and a library's pages under `docs/man/`. Those are the pages `doc` writes under `build/`, the one copy a checkout holds, mirrored at the release with their index as the README, so that a dependent's `lib/` holds the pages of the release it stands on. `CLAUDE.md`, the plan, the log, `docs/release.md` and `docs/full_review.md` are the way of working, and stay in the repository. `release` writes the archive's checksum beside it, `build/<name>-<version>.tar.gz.sha256`, and the two are published together.

**The installation.** `install`, from a checkout or an unpacked archive, puts what stands built under `PREFIX`, `/usr/local` by default, as Ernest's own `make install` does: the launcher in `bin/`, the compiled modules and `lib/` under `lib/<name>/`, and the documents under `share/doc/<name>/`, each at its path in the archive, so that the README's links resolve there. It builds nothing, so that an archive installs as it was compiled, replaces an installation already there whole, and refuses a launcher of another program's. `uninstall` removes exactly those, then `share/doc`, `share`, `lib` and `bin` under `PREFIX`, each where it is empty, and never `PREFIX` itself. A library has no launcher and nothing to install.

The source travels so that a consumer builds the modules with its own `ern`; the compiled modules travel so that an operator runs the application as it is, under any release of its floor. The `lib/` that travels serves the operator, for whom the archive is whole; a consumer lists every dependency itself.

## 5. The working rules

`CLAUDE.md` is a cut of Ernest's, in the same order. Most rules are kept as they are.

What changes is what the report shaped: the normative document is `docs/design.md` with the plan item being built, and the design changes first; where the design is silent, the sentence is added to it or the input refused; every section of the design has a test whose comment names it; a message that reports code work ends with *Design conformance*; a defect or a gap of Ernest's goes to `language_feedback.md` and what needed it waits, never worked around, but for a function Ernest can express; the program is Ernest, and `foreign` is only what the host alone can do.

Dropped: the soundness paragraph and the fixed section numbers, since the design is not cited by number from outside, and Ernest's reviews, replaced by `release.md`'s readers and `full_review.md`'s four.

Two rules keep the project's history out of what a user and a reader of the code see. User-facing text, the README, the manual pages and what the program prints, names no milestone, plan item or date of the project's history; a library's `since` line is the exception. A comment names no milestone, plan item, review finding or date, and cites the design's section and the log entry by its title instead.

A copy takes the file whole but for its title and the sentence under it, which says what the program is, so no row and no rule differs between the copies.

## 6. The release

`docs/release.md`: a fresh clone builds and passes; a cold reader over the README and the program, and from the release on which the program is first recommended to others a code reader over `src/` against the design and the principles; the findings fixed, planned or dropped; the version; the tag; the archive and its checksum, published so that another repository's `make lib` can name the archive; the note; and `language_feedback.md`'s lines carried to Ernest.

The tag is signed, `git tag -s`, with an SSH key GitHub holds as a signing key, so that GitHub marks it verified.

The note is the release's section of `CHANGES.md`, which the release step copies as the release's text on GitHub. It says what the release is and what a program or an operator of the previous release changes. Then comes one line a change, naming the design's section that states it. Its date stands in its heading alone, and it names no log entry, review or milestone.

`docs/full_review.md` is cut from Ernest's as `CLAUDE.md` is: four readers over the whole repository, a cold one who uses the program, one over all the code, one over the documents, and a security reader where the program takes input from outside. It runs only on the user's word, so a small program pays nothing for it. What a reader finds of Ernest's goes to `language_feedback.md`. A copy adds the readers its program alone needs.

## 7. What the template asks of Ernest

The rules an application follows are read from Ernest's installation, `guide/style.md` installed with the guide, and the template holds no copy, so that the rules have one owner. Ernest's own libraries stand on every job's load path, so they are not among `make lib`'s, and `--libs-dir lib` puts the Erlang applications on the load path. `ern test` runs a doc block's `// =>` examples (§11.2), so a library's page is held by its tests.

Two asks Ernest leaves to the program. A program's version is its own fact: a `let` held equal to `VERSION` by a test. Nothing resolves a dependency's dependencies, which Ernest leaves for later, so `DEPS` and `ERL_DEPS` are written in build order (section 4).

## 8. What the template does not do

It does not ship an empty file or directory. It does not copy Ernest's EUnit, its language-only documents or the readers of its reviews that read the language. It does not invent a dependency tool. It does not run in a continuous-integration service: a workflow would have to install OTP 29 and build Ernest before the application's seconds of tests, and a release archive of Ernest that installs without a build would change that.

It does not let the rules live in two places: an application is a copy, and what an application learns goes back here and from here into each copy, and into Ernest's `CLAUDE.md` where it applies there; `CLAUDE.md`, `tools/docs.ern` and `docs/full_review.md` are refreshed in an application by taking the template's again, the first but for its title and the sentence under it and the last but for the readers the application added, and the rules an Ernest program is written by are read from Ernest's installation, never copied.

## 9. How it is used

The repository is a GitHub template repository: *Use this template* makes the copy, and `README.md`'s last section says the six steps a copy takes. The last step removes `TEMPLATE.md` and `TEMPLATE_LOG.md`, which are the template's own. The template is tagged when the way of working changes, and the copy's first log entry names the tag.
