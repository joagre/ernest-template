# The template's design

What `ernest-template` is, why each of its files is there, and what each application begun from it has taught it. This is the template's own document and not a copy's: the last step of `README.md` removes it. It changes with the template, and a lesson from an application is a dated line of its last section. The design was proposed and decided in Ernest's repository on 2026-10-20, `docs/proposals/ernest_template/` there until it moved here, and built the same day.

## 1. What it is for

An application written in Ernest is not the language. It has no report of its own, no compiler, no Erlang of its own, no twelve readers, and no section numbers for tests to cite. What it shares with Ernest's repository is the way of working: a plan that says what is built and when, a log that says why, a proposal discussed until it is solid, a test before every commit, a read-back before a report, a stop after each item, and the owner of each fact decided before a sentence is written.

The template holds that way of working in a form small enough that a new application starts from it in one copy and one edit. It is a template and not a framework: it holds no code of its own but a launcher and one checker, and it decides nothing about the program's design. A library starts from the same template, with no `main` and no launcher.

The applications are where the language is used in anger. Each keeps `language_feedback.md` under `docs/` in the shape of Ernest's file of that name, a queue: a line is carried there by copy and then goes, and the file goes when it is empty, Ernest's file being the record; that road back is the template's reason to exist.

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

A file is in the template only where it has content on the first day. `README.md`, `CLAUDE.md`, `LICENSE`, the Zero-Clause BSD license as Ernest's own, which the README names, `VERSION`, `Makefile` and `.gitignore` at the top; `bin/name`, the launcher, renamed for the program on the copy.

`src/name.ern` is the entry module, a placeholder the copy renames and writes, so that the template's own `make test` is green and a copy begins green. `tools/docs.ern` is the checker, a source root of its own built into `tools/build/` and outside the archive.

Under `docs/` stand `plan.md`, `log.md`, `design.md` and `release.md`. The rules an Ernest program is written by are not among them: they are Ernest's `guide/style.md`, installed beside `ern`, which `CLAUDE.md` names and a session reads from the installation.

What appears when needed, named in `CLAUDE.md` so that nothing waits for a decision about where it goes: `language_feedback.md` at its first line and `findings.md` while a review's findings are open, both under `docs/`; `docs/proposals/` with the first proposal; `test/`, a second source root for a program run end to end, built into `test/build/`; `erl/`, one read-only git submodule per Erlang application the program stands on, pinned and never a copy.

Also when needed: `THIRD_PARTY_LICENSES` with the first borrowed file, an Erlang application under `erl/` among them, since the archive carries its compiled code, and `ACKNOWLEDGMENTS.md` with the first name; for a library, `examples/`, a source root built into `examples/build/` whose every program `make test` runs with one argument, `build/examples/<name>` and the Makefile's `EXAMPLE_SUFFIX`, and `docs/man/`.

Not committed: `build/`, each root's `build/`, `lib/` and `.ernest/`.

## 4. The Makefile, the launcher and the archive

One Makefile at the top, its variables first, `NAME`, `ERN_VERSION`, `DEPS` and `ERL_DEPS`, and the same nine targets in every application: `all`, `test`, `format`, `doc`, `man`, `run`, `lib`, `release` and `clean`. `man` mirrors the pages `ern doc` wrote into `docs/man/`, as Ernest's `make man` does, which a library's release commits. There is no light run and no full run, since an application's whole suite runs in seconds, and where one day it does not, that is a defect of the tests to measure.

**The load path.** The libraries of Ernest's own stand on every job's load path by the toolchain's own rule (§11.1, §11.2). Everything else a program loads beyond the standard library stands under `lib/`, which `make lib` fills: `lib/<name>/build` for a dependency, a release archive fetched by its URL and unpacked once; `lib/<app>/ebin` for an Erlang application built by its own `make` under `erl/`, its `priv` linked beside it. The load path is `lib/*/build` for a dependency's modules and `--libs-dir lib` for the Erlang applications, in the Makefile and the launcher both, and no path is written twice.

`DEPS` and `ERL_DEPS` are in build order, a dependency before what needs it; the template resolves nothing, which is Ernest's decision for another day.

**The build.** `all` checks the floor, fills `lib/`, builds each dependency's `src/` into its own `build/` with the consumer's own `ern`, and then the program's `src/`.

**The floor.** `version` compares the first two numbers of `ern --version` with `ERN_VERSION` and refuses another floor with both texts; a development build of the floor passes, since the applications are written against a checkout's `ern` to drive the language. `release` refuses a development build.

**The launcher.** `bin/<name>` runs `ern run` on the module its own name names with each `lib/*/build` and `--libs-dir lib` relative to its own directory, from a checkout and from an unpacked archive alike. It forwards a leading `--config-dir dir`, the one option an operator gives, and everything after it to the program; the working directory stays the caller's.

**The archive.** `release` runs `test`, then writes `build/<name>-<version>.tar.gz`: the launcher where there is one, `src/`, `build/`, `lib/` with each link copied through, the README, the license and `THIRD_PARTY_LICENSES` where there is one. One shape for an application and a library, so that any archive can be a dependency.

The source travels so that a consumer builds the modules with its own `ern`; the compiled modules travel so that an operator runs the application as it is, under any release of its floor. The `lib/` that travels serves the operator, for whom the archive is whole; a consumer lists every dependency itself.

## 5. The working rules

`CLAUDE.md` is a cut of Ernest's, under about a hundred lines, in the same order. Most rules are kept as they are.

What changes is what the report shaped: the normative document is `docs/design.md` with the plan item being built, and the design changes first; where the design is silent, the sentence is added to it or the input refused; every section of the design has a test whose doc block names it; a message that reports code work ends with *Design conformance*; a defect or a gap of Ernest's goes to `language_feedback.md` and what needed it waits, never worked around; the program is Ernest, and `foreign` is only what the host alone can do.

Dropped: the soundness paragraph, the revision date and the fixed section numbers, since the design is not cited by number from outside, and the three reviews, replaced by `release.md`'s two readers.

## 6. The release

`docs/release.md`, in six lines: a fresh clone builds and passes; two readers, a cold one over the README and the program and a code reader over `src/` against the design and the principles; the findings fixed, planned or dropped; the version, the tag and the archive, published so that another repository's `make lib` can name it; notes that list none of the changes; and `language_feedback.md`'s lines carried to Ernest.

## 7. What the template asks of Ernest

Lines 119 to 122 of Ernest's `language_feedback.md`, under its `docs/`: the style rules an application follows are not installed; a program cannot ask where Ernest's libraries are; a program cannot know its own version; and nothing resolves a dependency's dependencies.

The first two are answered on Ernest's `main` since 2026-10-21, and taken here 2026-10-22. The rules are read from Ernest's installation, `guide/style.md` installed with the guide, and the template's copy went, so that the rules have one owner. Ernest's own libraries stand on every job's load path, so they come off `make lib`, and `--libs-dir lib` puts the Erlang applications on the load path. The template therefore requires Ernest's `main` until 0.5.0 is tagged, while its floor says 0.4, decided with the user 2026-10-22.

## 8. What the template does not do

It does not ship an empty file or directory. It does not copy Ernest's EUnit, its reviews or its language-only documents. It does not invent a dependency tool. It does not run in a continuous-integration service: a workflow would have to install OTP 29 and build Ernest before the application's seconds of tests, and a release archive of Ernest that installs without a build would change that.

It does not let the rules live in two places: an application is a copy, a copy is never updated from the template, and what an application learns goes back here by hand and from here into the next copy; `tools/docs.ern` is refreshed in an application by copying the file again, and the rules an Ernest program is written by are read from Ernest's installation, never copied.

## 9. How it is used

The repository is a GitHub template repository: *Use this template* makes the copy, and `README.md`'s last section says the five edits a copy makes. The template is tagged when the way of working changes, and the copy's first log entry names the tag.

## 10. What the applications taught it

- *2026-10-20, `ernest-epx`, `v0.2.0`.* An Erlang application is not a dependency `make lib` fetches: epx is Erlang with a NIF and its own Makefile, tree_db beside it. An Erlang application is a read-only git submodule under `erl/`, named in `ERL_DEPS`, built by its own `make` and linked as `lib/<app>/ebin` and `priv`; the load path gained `lib/*/ebin`. rebar3 was set aside: epx's port configuration is rebar2's, its dependency unpinned, the tool absent. Tried before being written: a pixmap made, filled and read through the NIF from a scratch Ernest program.
- *2026-10-20, `v0.3.0`.* This document, moved here from Ernest's proposal, since a record that changes with the template has the template as its owner.
- *2026-10-20, `ernest-epx`, `v0.4.0`.* `make test` builds and runs `examples/` where it exists, each program given one output path; `make lib` links an application's `priv` only where it has one, which tree_db has not; and a test names its design section in a comment, since a doc block put every test on the module's page.
- *2026-10-20, `ernest-epx`'s release review.* The first run of `release.md`: a fresh recursive clone passed in a minute; two readers, an Opus 5.5 session each at high effort, a cold one over the README, the examples and the page and a code reader over the module against the design and the shape rules, handed in thirty-six findings, sorted in `findings.md` with a verdict each.
- *2026-10-20, the same review.* What it taught the template: `make` says when no `ern` is on `PATH`; the checker heads its list of long paragraphs as a notice, since a bare line read as a failure; the Makefile's lines are kept within 100 characters and a variable's comment stands on its own line, since make keeps the spaces before `#` in a value; and a tool that runs a doc block's `// =>` examples is wanted by every library, which no release has yet, Ernest's `language_feedback.md` 127.
- *2026-10-20, `ernest-epx`, `v0.6.0`.* The archive distributes what `erl/` builds, so `THIRD_PARTY_LICENSES` names each Erlang application's license and travels in the archive, and a release's notes name the application's commit and the platform the archive was built on.
- *2026-10-21, `v0.7.0`.* A built proposal is kept until its milestone's row names the log entries that argue it and nothing cites it, and goes after a reading, decided with the user, of what it holds that no owner has yet; Ernest's rule of the same day, so that the two repositories sweep alike.
- *2026-10-20, the same review.* The archive serves the operator and not a consumer, and a library's README says so. An application's `language_feedback.md` is a queue, emptied as its lines are carried, since a line in both files would have two owners. The checker reads no path in `plan.md` or `findings.md`, which name what is not written yet, as Ernest's own document test has it.
- *2026-10-20, `ernest-epx`.* A library's release commits its manual pages, as Ernest's does: `make man`, and `release.md`'s fourth line. The checker reads no path in `docs/man/`, whose pages `ern doc` writes.
- *2026-10-22, `ernest-epx`, planned.* A design's section numbers are cited by every test's comment and by doc blocks, eighty-three times in epx, and nothing holds them, so a section inserted in the middle leaves every citation pointing at the wrong rule with the tests green. The checker gains the check both ways: every `design §n` in `src/` and `examples/` names a section `docs/design.md` has, and every section is named by a test, as CLAUDE.md's *Tests* asks. Built here first, then copied into each application.
