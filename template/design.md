# The template's design

What `ernest-template` is, and why each of its files is there. This is the template's own document and not a copy's: the last step of `README.md` removes it. It states the design as it stands, and changes with the template. The template's history, where each rule came from and what each application taught it, is `template/log.md`'s.

## 1. What it is for

An application written in Ernest is not the language. It has no report of its own, no compiler and no readers of a language. What it shares with Ernest's repository is the way of working: a plan that says what is built and when, a log that says why, a proposal discussed until it is solid, a test before every commit, a read-back before a report, a stop after each item, and the owner of each fact decided before a sentence is written.

The template holds that way of working in a form small enough that a new application starts from it in one copy and one edit. It is a template and not a framework: it holds no code of its own but a launcher and one checker, and it decides nothing about the program's design. A library starts from the same template, with no `main` and no launcher.

The applications are where the language is used in anger. Each keeps `language_feedback.md` under `docs/` in the shape of Ernest's file of that name, its lines carried to Ernest and kept as `CLAUDE.md`'s *The work* says; that road back is the template's reason to exist.

## 2. What an application needs of the toolchain

Everything the template does, the toolchain does already; the template only chooses the roots and names them once.

- A directory that holds `package.conf` is a package, and the root package of every job started there (report §11.9). `ern build src` compiles every module under its `src/`, mirroring the tree into `build/`, in dependency order, and does nothing for a module whose source and dependencies have not changed (§11.1). Another source root, `tools/`, `test/` or `examples/`, compiles beside its source without `--build-root`, so the Makefile names its two roots.
- `package.conf` names the least release of `ern` the program is written for, which `ern build` holds the running `ern` to, and every package the program loads, by its name, its version, the URL of its archive and its digest. `ern unpack` unpacks each archive put under `lib/` there, `ern build` builds each package before the program, and every job started in the package puts each on the load path (§11.9). No job touches the network.
- A module's namespace is its path under the source root (§4.2). Each directory between a load-path root and a module is lowercase words joined by `_`; the root's own name is not checked (§11.1, §11.2).
- A test is a top-level `let` of type `Test.Case(m)` in the module it tests (Appendix E.24), and `ern test build` runs the tests of every module under the build root (§11.2), so unit tests live in their modules.
- `ern format --check` names each module not in the layout (§11.6); `ern doc` writes a module's documentation (§11.4).
- `--load-path dir` is a root under which modules are found by namespace (§11.2), and `--libs-dir dir`, of `ern run`, `ern test` and `ern shell`, puts the `ebin` of each application under `dir` on the load path, so an Erlang module a `foreign fn` names is found there as a `.beam`, and, by the host's rule, a NIF's library from `priv/` beside `ebin/` (§8.4, §11.2); the report states that of a named package alone (§11.9). `--package-dir dir`, of the same three, names the root package where the job is not started in it (§11.9).
- A compiled module is tied to the `ern` that built it, and one compiled against another interface or another standard library is refused before anything runs (§11.1, §11.2); two patch levels stand on one floor (§8.7).
- A program becomes a node by being started with `--config-dir dir` (§8.3, §11.3), a directory that holds the node's private key, `private-key.pem`, which `.gitignore` keeps out of a commit. The operator's side is the deployment guide's, and the template restates none of it.
- Until 1.0 a release of `ern` may refuse a program the previous release accepted, so `package.conf` names the least release the program is written for, a later release may refuse it until the program rises to it, and the program rises by its own session.

## 3. The tree

A file is in the template only where it has content on the first day. `README.md`, `CLAUDE.md`, `LICENSE`, the Zero-Clause BSD license as Ernest's own, which the README names, `CHANGES.md`, `VERSION`, `package.conf`, `Makefile`, `SECURITY.md` and `.gitignore` at the top; `bin/name`, the launcher, renamed for the program on the copy; and `template/`, this note and the template's log, which a copy removes.

`README.md` says what the program is for its reader and what it does, shows it once before *Building*, and then says where to begin, with central links only and no argument the program's own documents make. The showing is a picture, a session, or a few lines of the program's source. An Ernest block of the README is quoted and never written for the page: each of its parts, cut at its blank lines, stands in a tracked module once the module's comment lines are taken out, which `tools/docs.ern` holds. Under its title stands the epigraph, *The Importance of Being Ernest*, the line every application begun from the template keeps. The template's own README names the template in a line under the epigraph, since its top is the form a copy fills, and a copy removes that line.

`docs/README.md` says what each document is. `SECURITY.md` says where a security hole goes, and GitHub shows it in the repository's *Security* tab; the setting that takes such a report is not copied with the template, so a copy turns it on.

`.github/ISSUE_TEMPLATE/` holds a defect's issue form and a `config.yml`. The `config.yml` turns blank issues off and sends a security hole to private reporting. A copy changes the repository's address in it. The template's own `rule.yml` is the form a copy's rule comes back by, and a copy removes it.

`assets/` holds the repository's icon, 128 by 128, and its social preview on GitHub, 1280 by 640, with a README saying what each is. GitHub takes the preview from the repository's settings, so a copy replaces both pictures with its own and uploads its preview there.

`src/name.ern` is the entry module, a placeholder the copy renames and writes, so that the template's own `make test` is green and a copy begins green. Where every module stands is `docs/build.md`'s. Its one test's comment cites every section of the starter design until real tests do. `tools/docs.ern` is the checker, a source root of its own built into `tools/build/` and outside the archive.

Under `docs/` stand the documents `docs/README.md` names. The rules an Ernest program is written by are not among them: they are Ernest's `guide/style.md`, installed beside `ern`, which `CLAUDE.md` names and a session reads from the installation.

What appears when needed, named in `CLAUDE.md` so that nothing waits for a decision about where it goes: `language_feedback.md` and `known_issues.md` each at its first line and `findings.md` while a review's findings are open, all under `docs/`; `docs/proposals/` with the first proposal; `test/`, a second source root for tests run end to end, modules of tests that run the program with the checkout as their working directory, built into `test/build/`; `erl/`, one read-only git submodule per Erlang application the program stands on, named as the application, pinned and never a copy. The template's own `language_feedback.md` and `findings.md` stand while they hold lines, and a copy removes them; its `known_issues.md` holds the checker's, which a copy keeps with the checker.

The log is `docs/log.md` until it nears 256 KB, and then `docs/log/`, which the copy's session splits by day once; a repository tracks one form, never both. `docs/log/README.md` holds what stood above the entries, then `## Index`, a paragraph a day of one line, newest first, the days a blank line apart: `**2026-11-13.** [Title](2026-11-13.md#anchor); [Title](…)`. Each `docs/log/<date>.md` holds the entries whose first paragraph opens with its date, as they stood and in their order, under the heading `# <the log's title>, <date>`. `tools/docs.ern` holds both forms.

Also when needed: `THIRD_PARTY_LICENSES` with the first borrowed file, an Erlang application under `erl/` among them, since the archive carries its compiled code, and `ACKNOWLEDGMENTS.md` with the first name; `deploy/`, what an operator of the program reads, which an archive carries; and for a library, `examples/`, programs that use it, which `docs/build.md`'s *The examples* runs.

Not committed: `build/`, each root's `build/`, `lib/`, the packages' archives among it, `stage/`, where a release stages its archive, and a node's key, `private-key.pem`.

## 4. The Makefile, the launcher and the archive

`docs/build.md` states them: the Makefile and its targets, the launcher, the archive and the installation, the same in every application. A copy keeps the page, since its Makefile and its launcher are the template's.

## 5. The working rules

`CLAUDE.md` is a cut of Ernest's, in the same order. It holds what judgment cannot supply: what is the user's, who decides, and what the user wants of the work. It says nothing on how to think, and a mistake adds no rule to it.

Ernest's repository is upstream of the template. A change to the way of working is agreed with Ernest's session, by a message between the two sessions, and decided by the user. A rule Ernest holds comes to the template whole, never weighed part by part for an application, but for what this section says changes or is dropped.

What changes from Ernest's is what the report shaped. The normative document is `docs/design.md`, and the design changes first. Where the design is silent, a sentence is added to it. Every section of the design has a test whose comment names it. A defect or a gap of Ernest's is a line of `language_feedback.md` and what needed it waits, never worked around, but for a function Ernest can express over what the library has. A corner that only a built program meets is a line of `known_issues.md`.

Dropped: the soundness paragraph, the cold reading and the fixed section numbers, and Ernest's reviews, replaced by `release.md`'s readers and `full_review.md`'s four.

`tools/docs.ern` keeps the project's history out of what a user and a reader of the code see, holds a paragraph to 150 words, and holds the log to its form: the tool says so when one is broken, and the file states neither.

A copy takes the file whole but for its title and the sentence under it, which says what the program is, so no row and no rule differs between the copies.

`docs/agents.md` is cut from Ernest's page of that name: what a brief holds, where an agent's report goes, what is checked before agents start and after they end, and the model each job gets. `CLAUDE.md` keeps what goes to an agent, and has a session read the page before it starts its first. A copy takes the page whole.

## 6. The release

`docs/release.md` says what a release runs to be ready, the note's contents among it, in the order it runs them. The archive and its checksum are published so that another repository's `package.conf` can name the archive.

`docs/full_review.md` is cut from Ernest's as `CLAUDE.md` is: four readers over the whole repository, a cold one who uses the program, one over all the code, one over the documents, and a security reader where the program takes input from outside. It runs only on the user's word, so a small program pays nothing for it. What a reader finds of Ernest's goes to `language_feedback.md`. A copy adds the readers its program alone needs.

## 7. What the template asks of Ernest

The rules an application follows are read from Ernest's installation, `guide/style.md` installed with the guide, and the template holds no copy, so that the rules have one owner. Ernest's own libraries stand on every job's load path, so they are not among `package.conf`'s; the packages it names are found, checked, built and loaded by `ern` itself (§11.9), and `--libs-dir erl` puts the program's own Erlang applications on the load path. `ern test` runs a doc block's `// =>` examples (§11.2), so a library's page is held by its tests.

One ask Ernest leaves to the program. A program's version is its own fact: a `let` held equal to `VERSION` by a test. Nothing chooses a package's version: the root package's `package.conf` writes each, a package another loads among them, and `ern build` holds each package's own entries to them (§11.9).

## 8. What the template does not do

It does not ship an empty file or directory. It does not copy Ernest's EUnit, its language-only documents or the readers of its reviews that read the language. It does not invent a dependency tool, and fetches no package's archive, which its author downloads. It does not run in a continuous-integration service: a workflow would have to install OTP 29 and build Ernest before the application's seconds of tests, and a release archive of Ernest that installs without a build would change that.

It does not let the rules live in two places: an application is a copy, and what an application learns goes back here and from here into each copy, and into Ernest's `CLAUDE.md` where it applies there; the files `CLAUDE.md`'s *What is the user's* calls the template's are refreshed in an application by taking the template's again, as it says, and the rules an Ernest program is written by are read from Ernest's installation, never copied.

## 9. How it is used

The repository is a GitHub template repository: *Use this template* makes the copy, and `README.md`'s last section says the six steps a copy takes. The last step removes `template/`, the template's own design note and log, and its own issue form. The template is tagged when the way of working changes, and the copy's first log entry names the tag.
