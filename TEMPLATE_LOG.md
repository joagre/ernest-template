# The template's log

The template's own dated record, newest last: where each rule of `TEMPLATE.md` came from and what each application taught the template. A copy removes it with `TEMPLATE.md`. It is never normative: `TEMPLATE.md` states the design as it stands.

## The design, 2026-10-20

The template's design was proposed and decided in Ernest's repository, `docs/proposals/ernest_template/` there, and built the same day. Its section 7 asked four things of Ernest, Ernest's feedback 119 to 122: the style rules an application follows are not installed; a program cannot ask where Ernest's libraries are; a program cannot know its own version; and nothing resolves a dependency's dependencies.

Ernest's log, *What the Feedback Left*, decided them the same day. The style rules installed with the guide (119) and Ernest's libraries on the default load path (120) became items of Ernest's MVP 3.28. A program's own version (121) was left alone: a `let` held equal to `VERSION` by a test is the mechanism, and a version is the program's fact. Dependencies (122) went under *Later*.

## An Erlang application is a submodule, 2026-10-20

From `ernest-epx`, at the template's `v0.2.0`. An Erlang application is not a dependency `make lib` fetches: epx is Erlang with a NIF and its own Makefile, tree_db beside it. An Erlang application is a read-only git submodule under `erl/`, named in `ERL_DEPS`, built by its own `make` and linked as `lib/<app>/ebin` and `priv`; the load path gained `lib/*/ebin`.

rebar3 was set aside: epx's port configuration is rebar2's, its dependency unpinned, the tool absent. It was tried before being written: a pixmap made, filled and read through the NIF from a scratch Ernest program.

## The design note moves here, 2026-10-20

At `v0.3.0`, `TEMPLATE.md` moved here from Ernest's proposal, since a record that changes with the template has the template as its owner.

## The examples, `priv` and a test's citation, 2026-10-20

From `ernest-epx`, at `v0.4.0`. `make test` builds and runs `examples/` where it exists, each program given one output path. `make lib` links an application's `priv` only where it has one, which tree_db has not. A test names its design section in a comment, since a doc block put every test on the module's page.

## The first release review, 2026-10-20

`ernest-epx`'s release review was the first run of `release.md`. A fresh recursive clone passed in a minute. Two readers, an Opus 5.5 session each at high effort, a cold one over the README, the examples and the page and a code reader over the module against the design and the shape rules, handed in thirty-six findings, sorted in `findings.md` with a verdict each.

What it taught the template: `make` says when no `ern` is on `PATH`; the checker heads its list of long paragraphs as a notice, since a bare line read as a failure; and the Makefile's lines are kept within 100 characters and a variable's comment stands on its own line, since make keeps the spaces before `#` in a value.

A tool that runs a doc block's `// =>` examples was wanted by every library, Ernest's feedback 127. Ernest built it the next day, under `ern test` (Ernest's log, *What the Feedback Left*).

## The archive serves the operator, 2026-10-20

From the same review. The archive serves the operator and not a consumer, and a library's README says so. An application's `language_feedback.md` is a queue, emptied as its lines are carried, since a line in both files would have two owners. The checker reads no path in `plan.md` or `findings.md`, which name what is not written yet, as Ernest's own document test has it.

## A library's manual pages, 2026-10-20

From `ernest-epx`. A library's release commits its manual pages, as Ernest's does: `make man`, and `release.md`'s fourth line. The checker reads no path in `docs/man/`, whose pages `ern doc` writes.

## The licenses travel, 2026-10-20

From `ernest-epx`, at `v0.6.0`. The archive distributes what `erl/` builds, so `THIRD_PARTY_LICENSES` names each Erlang application's license and travels in the archive. A release's notes named the application's commit and the platform the archive was built on.

## A built proposal goes, 2026-10-21

At `v0.7.0`. A built proposal is kept until its milestone's row names the log entries that argue it and nothing cites it, and goes after a reading, decided with the user, of what it holds that no owner has yet. It is Ernest's rule of the same day, so that the two repositories sweep alike.

## The style rules and the libraries from the installation, 2026-10-22

Ernest's `main` answered the first two asks on 2026-10-21, and the template took them on 2026-10-22. The rules are read from Ernest's installation, `guide/style.md` installed with the guide, and the template's copy went, so that the rules have one owner. Ernest's own libraries stand on every job's load path, so they came off `make lib`, and `--libs-dir lib` puts the Erlang applications on the load path. The template required Ernest's `main` while its floor said 0.4, decided with the user the same day.

## The design's citations held, 2026-10-22

From `ernest-epx`. A design's section numbers are cited by every test's comment and by other comments, eighty-three times in epx, and nothing held them. A section inserted in the middle left every citation pointing at the wrong rule with the tests green.

The checker holds them both ways: every `design §n` in a comment under `src/`, `test/` and `examples/` names a section `docs/design.md` has, and every section is named by a test's comment, a doc block not among them, as CLAUDE.md's *Tests* asks. It was built here first, then copied into each application.

## A recursive clone, 2026-10-23

From `ernest-epx`'s second review. The release checklist's clone is `--recursive` where there is an `erl/`, since a plain clone stops at an empty submodule. The Makefile's header names the design's citations among what `make test` checks.

## Five rules from Ernest's, and the floor 0.5, 2026-10-25

Taken from Ernest's `CLAUDE.md`: a session opened to discuss alone names each write before it is made; a finding is argued after the log and the program; a shim is written with the host's page open; an undiagnosed defect is planned with the shape of its fix; and a step sweeps what it leaves behind.

`release.md` took the same day the cold reader's round over the review's own diff, the two models, the `since` of a new declaration, and the notes' two lines on where what changed is read and what the review did not run.

Ernest 0.5.0 was tagged the same day, and the floor became 0.5. Ernest 0.6.0 was tagged the same night.

## A refusal weighed, and the floor 0.6, 2026-10-27

Taken from Ernest's: a refusal the design states is weighed on the principles, and a sentence that teaches a way around the program or Ernest is a gap. The floor became 0.6.

## The floor 0.8, 2026-11-01

The floor became 0.8, for the pun, `=f` for `f = f`, which Ernest's checkout wrote as it worked toward 0.8.0 and 0.7 refuses.

## The floor 0.9, 2026-11-02

The floor became 0.9, for the archives Ernest's checkout makes toward 0.9.0. Each says its commit, `0.9.0+<commit>`, and an application built clean-room installs one.

## The examples run in one word, 2026-11-02

From `ernest-epx` and `ernest-httpd`. `make examples` builds every program of `examples/` and runs each, what it writes under `build/examples/`, and `make test` runs it after its own checks. A reader builds and runs the examples in one word, which the README says in place of a shell loop, and the Makefile's loop is written once.

A program of `examples/` is an `.ern` file at its top, from httpd, whose example is a site of data under it. So a directory with no program is laid out, built and run by nothing.

## Install and uninstall, 2026-11-02

From `ernest-httpd`'s first release. Its cold reader ran the README as a user, and found the archive `make run` could not run in and the installed README whose links led nowhere. The template gained `make install` and `make uninstall`, as Ernest's own, and the launcher's root rule, one file for a checkout, an archive and an installation. The archive carried the Makefile, `VERSION` and the tracked documents, so that it runs and installs as it unpacks.

The checker reads a backticked text that holds a space as a command line and not a path. The README's usage line, `bin/<name> [--config-dir dir] config.json` with the program's name, was refused as a path that does not exist and had to stand in a fence.

## A development build by `+`, 2026-11-05

From `ernest-httpd`. `release` knew a development build only by `-dev`, so an archive's `ern 0.10.0+612faac8`, which the report's §11.7 calls no release, passed. It refuses `+` as well, which a `.dirty` build also carries.

## Cut again from Ernest's redraft, 2026-11-06

`CLAUDE.md` was cut again from Ernest's redraft, in its plain register, a chain of clauses split into sentences (Ernest's log, *The Template Cut Again*). A proposal refused or not taken up stays. The owner table names `docs/README.md` once for the documents under `docs/`. A good rule found in an application goes to the template, and from it to the other copies and to Ernest's file. A new file is added before its check runs, a flake is tested under what it was seen under, a proposal's pause pushes, and a log is split by day before GitHub stops rendering it.

One gap of Ernest's stopped waiting: a function the library lacks, which Ernest can express, is written in the program while its line waits. The file had said both that it is written and that nothing goes around a gap. `docs/full_review.md` came the same day, cut from Ernest's.

## An `ERN` that is a path, 2026-11-06

From `ernest-httpd`, its `e7cee6b`. `ERN=path/to/ern` reached the Makefile's own commands and not what names `ern` by its name. Two of its test cases failed with `ERN=` set and none on `PATH`, and with another first on `PATH` they ran that one.

The directory of an `ERN` that is a path stands first on `PATH` for every target, since principle 1 has a reader expect every `ern` the build starts to be the one named. A file not called `ern` is not reached so, as the Makefile and the README say. The template names `ern` so nowhere, the launcher reading `ERN` itself, so the line serves a copy's tests. It was run by hand, and no standing test holds it.

## The documents' check runs last, 2026-11-06

From `ernest-epx`, its `0fb5eb3`. The documents' check ran before `make examples`, so a document naming what an example writes by its full path was refused on a clean tree, and `make test` stopped before the example could write it. The check runs last in `make test`.

Principle 1 decided: one command on one tree gives one answer, and a true sentence is not refused. A full path is held against what was built, where the metavariable form is not checked. The checker leaving out `build/` was set aside, since it would drop that check and add an exception.

## The release cleanup, 2026-11-07

Ernest's four repositories were read as a stranger reads them before the launch (Ernest's log, *The Release Cleanup*). `TEMPLATE.md` states the design in the present, and its history, its section 10 of lessons among it, moved here. The template's `docs/log.md` is the placeholder every copy begins with, so the template's own history has this file.

An archive carries the user's documents alone, so `CLAUDE.md`, the plan, the log and the review checklists stay out of it. The release publishes a checksum beside the archive and signs its tag. The note says what the release is and names the design's section a change, and no log entry, review or milestone. The issue form came, with blank issues off and a security hole sent to private reporting.

Two rules came from Ernest's. User-facing text names no milestone, plan item or date, a library's `since` line excepted. A comment names no milestone, plan item, review finding or date, and cites the design's section and the log entry by its title. Ernest's report has no revision date any more, so the template no longer says it drops one.

## The rules held by the checker, 2026-11-07

The two rules and the note's form held by the read-back alone, so `tools/docs.ern` holds them (Ernest's log, *Holding the Release Cleanup*). A comment of a module, a line that begins `//`, names no milestone, plan item, review finding, feedback line or date. A line of the README, of `CHANGES.md` or of a module under `src/` names no milestone. A section of `CHANGES.md` holds no date outside its heading and no `; *Title*`, and names neither the plan nor a review, its reader or a newcomer.

The checks read lines and words, as Ernest's tests do. A first build read each module by its tokens and each form a character at a time, and doubled the checker; it was set aside for its size. A comment after code and a block comment are not read. A line under `src/` is read whole, its identifiers among it, since one that names a milestone is as wrong as a string that does. The README's step 3 named the plan's first milestone, which the check found, and it says `docs/plan.md` now.

What it costs is stated here and kept. On `ernest-httpd`, about 11,000 lines of Ernest, the checker took about 420 ms and takes about 600 ms, `String.words` and `String.trimStart` about 6 µs a line each. A filter that skipped lines holding none of the forms would win most of it back and was not written, since it is a second reading kept only for speed.

The release signs its tag with an SSH key GitHub holds as a signing key, since the pushes go over HTTPS and use none.

## The pictures, 2026-11-07

The template has an icon and a social preview under `assets/`, as ernest-epx and ernest-httpd have, with a README saying what each is, since nothing else names them. *Use this template* copies them into every new repository, so the README's step 6 has a copy replace them with its own.

## The archive carries the pictures, 2026-11-07

From `ernest-epx`, read after the release cleanup. Its archived `README.md` shows its collage under `assets/` and its examples' README each example's picture there, but the archive left `assets/` out, so every picture was a broken link in the archive and in an installation. Ernest's own archive copies the logo its README shows for the same reason. `DOCS` takes the files git tracks under `assets/`, so `make release` and `make install` carry them, the icon and the social preview among them, which no document shows but which cost a few hundred kilobytes. Carrying only the pictures a document names was set aside, since it would read every document's links to save that.
