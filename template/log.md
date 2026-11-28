# The template's log

The template's own dated record, newest last: where each rule of `template/design.md` came from and what each application taught the template. A copy removes it with `template/design.md`. It is never normative: `template/design.md` states the design as it stands. An entry before *Ernest agrees* names the two by their former names, `TEMPLATE.md` and `TEMPLATE_LOG.md`.

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

## The floor 0.10, 2026-11-10

Ernest 0.10.0 was tagged on 2026-11-10, and the floor became 0.10 the same day (Ernest's log, *The Release Review Before 0.10.0*). Ernest's plan had set the template's rise at its MVP 4.4's item 4, later. It came now because ernest-httpd's floor is 0.10 already, and a copy ahead of its template cannot take the template's files whole.

The template was run under 0.10.0 before it rose. One line changed: `tools/docs.ern`'s command for `git ls-files` is written `Os.command(program, arguments)`, since `Os.Command` gained `environment` and `workingDirectory`, and 0.9.0 has no `Os.command`, so no one line served both. 0.10.0's other three rules, a qualified name in its shortest form, `kill` taking a `Process` and a pipe into a parenthesized pipe, touch nothing in the template.

## One copy of the pages, 2026-11-11

From `ernest-httpd`. Sessions read signatures in `docs/man/`, which `make man` wrote at the last release, and so read contracts gone since: its `docs/man/smoke.md` still showed `Smoke.terminate(program, pid)` after the function had come to take the program alone. A rule sending sessions to the source or to `build/` instead was weighed and set aside. A copy stale by design under `docs/` surprises whoever opens it (principle 1), and a rule in prose that steers around it is a gap with its workaround beside it. A check in `make test` that kept `docs/man/` current was set aside too, since every change to a doc comment would then carry its pages twice.

The pages are `make doc`'s alone, under `build/`, the one copy a checkout holds (principle 2). `make release` mirrors a library's into its archive's `docs/man/`, its index their README, so that a dependent's `lib/` and an installation hold the release's own pages. `make man` went, and with it `release.md`'s commit of the pages and the checker's exemption of a tracked page. The mirror now leaves out what the examples write under `build/examples/`, which `make man` would have taken had an example written Markdown. A reader on GitHub loses the pages there and will read them on ernest-lang.org. This reverses *A library's manual pages*.

## The archive's sources, 2026-11-11

From `ernest-httpd`. `make release` copied `src/` whole, so an untracked file under it, and one git ignores, such as a stray `.erc` beside its source, went into the archive. The sources now go as the documents do: `SOURCES` names the files git tracks under `src/` in a checkout, and every file there in an unpacked archive, and the `tar` that copies `DOCS` copies them. `TEMPLATE.md`'s *The archive* says so. No test holds it, since `make release` runs `make test` first, and a test that ran the release from inside `make test` would recurse; the archive's sources are `git ls-files` by construction.

## The done line stays, 2026-11-11

From `ernest-epx`, which asked that a done item leave no line in the plan, since the line repeats *Where we are* and the log on a page read for what comes next. The rule stays: a done item's paragraph goes, and one line naming its log entries stands in its place until the milestone's row takes it.

Principle 2 decided, read whole. Until a milestone closes, the line is the one place that says which entries argue its finished items, and the row is written from it. epx's milestone 9 named four entries there, none of which names the milestone, so without the line its row would be rebuilt from dates in a log where other work interleaves, and a missed entry is caught by no test. Principle 1 audited: where a plan's items are a numbered list, the line holds its item's number. CommonMark counts on from a list's first number, so a gap renumbers the rendered list, and a citation of an item stops matching the page.

## The commands' comments, 2026-11-11

From Ernest, on the user's word, so that one form holds across the repositories. The README's block of make targets writes each description after `#`, and each line that continues one begins with `#` under the first, as Ernest's README and its `development.md` write theirs. A block of commands is shell that a reader pastes, and a bare description pastes as arguments: `make test` followed by its description asks make for targets named `the` and `layout,`. Principle 1 decided. A copy takes the template's line word for word for each target it shares, and writes its own only for a target of its own.

The checker does not hold the form. It cannot tell a block of commands from one of code or of output by its lines without guessing at the block's language, and the rules it holds are read exactly. The block is one in each repository and comes from the template whole.

## The commands held by the checker, 2026-11-11

This reverses the second half of *The commands' comments*: `tools/docs.ern` holds the form, as Ernest's style test does (its `shell_comment_test`). Ernest's test showed that a command is told by its first word, so the check guesses at no block's language. And the lines a copy writes for its own targets come from no template, so a read-back of the template's block would never see them. Where a check that costs cycles finds what a reader would, the check runs (`CLAUDE.md`, *The repository*).

The rule is Ernest's, for every fenced block but an Ernest one in the files whose paragraphs are measured. A command is a line that begins with `make`, or with `ern` or a launcher under `bin/` and a word, after an optional `sudo` and words `VAR=value`. It holds no two spaces before its `#`, and a line indented under it begins with `#`. A command that ends in `\` runs on to the next line. The line is cut at its first ` #`, so a comment with two spaces inside it reads as a comment. Two misses are accepted, since no document writes either: a `make` line in a block of another language is read as a command, and a ` #` inside an argument ends the command early. Ernest's test takes both of the template's departures from its own, so the two checks read one rule.

It caught every line of the block at `v0.10.1`, and found nothing on `ernest-epx` and `ernest-httpd`, whose blocks hold 13 and 12 commands. On `ernest-httpd` the whole checker took 772 to 795 ms against 750 to 817 ms without it.

## The rules read for clarity, 2026-11-15

From Ernest, whose `CLAUDE.md` was rewritten where a session could take a sentence two ways (Ernest's log, *The Rules Read for Clarity*). The template takes the reading in its own words, and is tagged `v0.10.4`.

**The agents' page.** The agents' rules move to `docs/agents.md`: the brief, an agent's report, what is checked before and after, and the models. `CLAUDE.md` keeps what goes to an agent and that its report is a claim, and has a session read the page before its first agent. The page is the template's and a copy takes it whole. `docs/full_review.md` and `docs/release.md` cite it for a reader's model. The cost is Ernest's: a pointer a session may not follow.

**The owners' table.** Three rows go. `README.md` and `SECURITY.md` own what their names say, and *Style* names Ernest's `guide/style.md` with its path. The row of `CHANGES.md` points at `docs/release.md`, whose sixth step already says what a note holds. The rows of `deploy/README.md` and `examples/README.md` stay, since each places a file the template does not hold yet.

**Rules that said two things.** The index was left as the user left it, while a new file was staged. A deletion was committed at once, under *Commit only after the checks pass*. A proposal's pause stood in *Tests* and in *Before code*. *Where the design is silent* let the code reject an input and add no sentence. Each says one thing now, as Ernest's does.

**One path for a gap.** The path is said once. A defect of the program's own is fixed or planned, and a gap of Ernest's is a line of `language_feedback.md`. The function Ernest can express stays the one gap that does not wait.

**Words with two meanings.** "The report" alone is Ernest's, and the session's is "the report to the user". The read-back is a diff read and the reading at an item's close. The checklist's lines each name their rule and no more.

**Not taken.** What has no counterpart here: the design note, *Ernest or Erlang*, the refusal made for a later release's sake, the two searches of the read-back, and the ladder a cost goes by, whose contradiction this file never held.

## A function over the library's types, 2026-11-15

From Ernest, whose sweep read every private function of its own programs and of the applications by one test (Ernest's log, *A Library's Function in a Program* and *The Sweep's Reading*). The template takes the rule in its own words, for what is written from now on, and is tagged `v0.10.5`.

**The test.** The rule on a function the library lacks fired on a feeling. Now a private function whose type names no type of the program's own is read against the admission rules of the report's Appendix E.0. Where a rule admits it, its line in `language_feedback.md` is written, and for no other function, so the queue gains no noise. The function is still written in the program meanwhile, and goes when a release brings the library's own. The reading is a first cut, since the installation holds the report, and the verdict stays Ernest's.

**The search.** The reading at an item's close searches the sources for such a function, and gives its count. *The rules read for clarity* left the two searches of the read-back out as having no counterpart here, and the test of the type gives this one its counterpart.

**Not taken.** The other search, for a form the code repeats. Nothing has yet argued it for an application, and it waits for that argument.

`TEMPLATE.md` §5 names the test where it names the function Ernest can express.

## The repeated form, 2026-11-15

The repositories keep the same rules: what Ernest's `CLAUDE.md` holds, the template holds in its own words, and a rule needs no argument from an application to come here. So the template takes the search for a form the code repeats, and is tagged `v0.10.6`. This reverses the *Not taken* of *A function over the library's types*.

**The gap.** A form the code repeats at site after site joins what writing Ernest feels against a principle, with the workaround, the second way and the function the library lacks. It is a line of `language_feedback.md` with its count, and the verdict is Ernest's.

**The two searches.** The reading at an item's close runs both, each over the sources with its count. In Ernest the search for a repeated form found the pun, at 190 sites, and two lines of its feedback (Ernest's log, *The Pun* and *The Sweep's Reading*).

## Two hours for a hunt, 2026-11-16

A flake's hunt gets a bound, taken from Ernest's `CLAUDE.md` in the template's words, and the template is tagged `v0.10.7` (Ernest's log, *Two Hours for a Hunt*).

**The rule.** A flake is hunted for two hours at most, under what it was seen under, and the hunt ends at its first sighting. One that does not show is closed as not reproducible, and opened again where it shows again. A probe that makes the failure at will shows the cause and the fix, and no hunt follows. Where none can, the hunt runs to its third sighting, and the hunt after the fix runs three times the runs one sighting took.

**Why.** A hunt must cost less than its flake does. Two hours is a budget, chosen and not measured. The rest is derived: one sighting shows that the hunt is the place, three give a rate, and three times a sighting's runs, run clean, leave about one chance in twenty that the flake still stands. In Ernest a hunt ran two hours before a fix and began two hours after it, where the flake had shown in the fourth minute and a probe had shown the cause.

## The review documents read against the rules, 2026-11-16

One reader read `docs/full_review.md` and `docs/release.md` at `8491145` against `CLAUDE.md` and `docs/agents.md`, beside Ernest's own two. The lines were decided with the user in Ernest's session, which wrote them here, and the template is tagged `v0.10.8` (Ernest's log, *The Review Documents Read Against the Rules*).

**The full review owns what the release pointed at.** `full_review.md` is the template's and took its clone step and its sorting from `release.md`, which each copy owns and one copy had already changed. Both are stated in `full_review.md` now, and `release.md` points there. A file the template gives rests only on files the template gives.

**A reader.** A reader is an agent, not a session. It is handed `CLAUDE.md` as every agent is, which a probe showed, so its brief stands in place of it, and `agents.md` names the exception. A reader held truly cold would be a session of its own outside the checkout, for the little `CLAUDE.md` gives away. The stronger model reads at the session's own effort. The list of what a reader finds of Ernest's follows `CLAUDE.md`'s, the repeated form among it.

**A fix.** Who makes a fix is said once, with the sorting. An agent runs the program or the command a finding gives before it makes the fix, and hands back a line that does not fail, so that no fix is built on a failure nobody saw.

**The release.** Its readers are the full review's K and C, run as it runs them, where step 2 restated them narrower. The round's cold reader reads the diff of what it reads, and the session reads the code's lines back. The note stands before the release step, since it is committed before the tag. The push and the release on GitHub wait for the user's word.

The step for the milestone's proposal went. `CLAUDE.md`'s *Proposals* has an item of the milestone remove the directory before the release, and the step did it after the tag.

## A reader's brief says that it stands in place, 2026-11-16

`full_review.md` says that a reader's brief stands in place of `CLAUDE.md`. It now says that the brief tells the reader so in one line, and the template is tagged `v0.10.9` (Ernest's log, *The Review Documents Read Against the Rules*).

**Why.** `CLAUDE.md` says of itself that it overrides, and a reader has it in its context. A brief that does not say it stands in its place leaves the promise to the session's memory. The first review under the sentence shows whether a reader keeps to its brief: a cold reader that cites the log or a rule of `CLAUDE.md` is the sign.

## Hard work and stupid work, 2026-11-16

`CLAUDE.md`'s *Done* says that work is never left for its size, taken from Ernest's `CLAUDE.md`, and the template is tagged `v0.10.10` (Ernest's log, *Hard Work and Stupid Work*).

**The rule.** Nothing is left, or recommended left, for its size or its difficulty: where it is right it is done in the item, or planned. Work is left only where it would hold nothing, decide nothing and remove nothing, and the reason given is that one, never the cost.

**Why.** The rules said to decide every surprise, to act on it or leave it with its reason, and no rule said which reasons count. In Ernest a session closed an item and recommended three things left: some forty sites that wrote by hand what the item's new helper named, an answer that two like cases gave in two ways, and two paths without a test. Its reason each time was the work. Each was worth doing, and the three recommendations were taken back the same day. The other half keeps the rule from asking for work by rote: a tidy, a test or a measurement that would hold nothing, decide nothing and remove nothing is not done, however small.

## The front page shows the program, 2026-11-16

The README's form asks for one showing before *Building*, `tools/docs.ern` holds an Ernest block of the README to the program's modules, the template's own README says under its title what it is, and the template is tagged `v0.10.11` (Ernest's log, *The Front Page in the Announcement's Manner*).

**The form.** The form's top asked for what the program is and where to begin, in a paragraph. Both applications followed it, and each page went from one sentence to *Building* and showed nothing. Ernest's own front page was written again to say what Ernest does and show it, and the two applications' pages followed the same day. The form now asks for what they hold: what the program is in a sentence a stranger can read, what it does, and one showing, a picture, a session or a few lines of the program's source. It still makes no argument the program's documents make.

**The check.** A page that quotes the program can drift from it, and nothing held the two equal. Each part of a block fenced as `ernest` in `README.md`, its lines between blank lines, must stand as consecutive lines, compared whole, in one tracked module under `src/`, `test/` or `examples/`, once that module's comment lines are taken out. A part that stands nowhere is named by its first line, and `make test` fails.

The rule needs no mark in the page and no path beside the block. It also says more than equality: an Ernest block of the README is never written for the page, so what a reader copies from it has been compiled, and run where it stands in an example.

**The template's line.** The template's README is the form a copy fills, so a visitor met `# NAME` and a placeholder, and learned what the repository is in the last section. A line under the title says it now, and the copy's last step removes the line.

**In the tool.** The check asks whether a part's lines stand in a module's text, through `String.contains` over both texts with a line break before and after, which is the rule as it is stated and no way around a search the library lacks. The place a finding's line begins with, the file and the line, stood written out at five sites and is one function, `placeOf`. The tool's tests carry doc blocks where `CLAUDE.md` asks a test's comment to be none; `tools/` has no page, so the sentence's reason does not reach it, and they stay.

## A plan's item and the user's idea are steps too, 2026-11-17

`CLAUDE.md`'s rule for a step that looks wrong covers a plan's item and the user's own idea, before the work starts, taken from Ernest's `CLAUDE.md`, and the template is tagged `v0.10.12` (Ernest's log, *Twenty-Six Hosts Are the Cost*).

**The rule.** A plan's item and the user's own idea are steps too: before work starts on one, say whether it is worth doing, and say no where it is not.

**Why.** The rule read as one for a step met while building, and an item that stands in the plan read as decided. In Ernest a plan's item named the cost of the repository's own make. An evening went to measuring it and to a build that was stopped unfinished, before anyone asked who pays that cost. Only who builds Ernest from source does, so nothing was built. The question belonged before the first measurement, and the plan's word, or the user's, does not answer it.

## The session's own suggestion is a step too, 2026-11-17

`CLAUDE.md`'s rule for a step that looks wrong names a suggestion of the session's own beside a plan's item and the user's own idea, taken from Ernest's `CLAUDE.md`, and the template is tagged `v0.10.13` (Ernest's log, *The Session's Own Suggestion*).

**The rule.** A plan's item, the user's own idea and a suggestion of the session's own are steps too: before work starts on one, say whether it is worth doing, and say no where it is not.

**Why.** The sentence of `v0.10.12` named two cases, and a session that had it weighed a plan's item before it started the item. The same session made suggestions of its own that it had not weighed, a rule change among them, and took each back when asked whether it recommended it. A recommendation is what a session is for, and one made unweighed costs the trust in the next. The sentence worked where it named the case, so it names this one.

## Agents bound by the processor run one at a time, 2026-11-17

`docs/agents.md`'s *The brief* says that agents whose work is bound by the processor run one at a time, which the template's issue 2 asked for out of ernest-epx, and the template is tagged `v0.10.14`.

**The rule.** Agents whose work is bound by the processor, a race's probe, a run under a sanitizer or a load test, run one at a time, and each runs its programs one after another: side by side is for work that waits or reads. The brief says so.

**Why.** `CLAUDE.md` sends work that can run side by side to agents, and nothing said which work that is. In ernest-epx three agents were started side by side, each to write and run race probes: programs of two or three processes in tight loops, each run four times on two builds, one of them under the address sanitizer. Each agent ran its programs overlapping, an Erlang node of 24 schedulers apiece. The load of the 24-core machine, which is also the desktop the work is read on, passed 200 and stayed high for about an hour. One run at a time would have found the same. *The tools are fast* measures one run against its work, and says nothing of three at once.

**What was left out.** The issue also asked that the first message to the user say how many cores the run takes and for how long. One run at a time leaves little to announce, and a session seldom knows the duration before the run. `CLAUDE.md` gets no pointer, since it already has a session read the page before its first agent.

## The load another session makes, 2026-11-17

`docs/agents.md`'s *The brief* has a session read the machine's load before it starts an agent whose work is bound by the processor, which Ernest's session sent back when it agreed to the sentence of `v0.10.14`, and the template is tagged `v0.10.15` (Ernest's log, *What Waits for a Peer*).

**The rule.** A session reads the machine's load before it starts such an agent: a load another session makes is said to the user, who says whether the agent waits.

**Why.** The sentence of `v0.10.14` binds the agents of one session, and the machine is shared by several. A load test or a flake's hunt fills the machine even where it runs alone, and a second session that starts its own agent on top adds to the load and skews its own timings. In Ernest a timing test failed once in a full run while two other repositories' sessions ran a load and a hunt, the five-minute load at 69 on 24 threads. Reading the load costs one command.

**The user says whether it waits.** The wording sent said that such a load is waited out. A session cannot know how long another session's work runs, and a wait with no deadline is one nobody decided. The user knows what the other sessions do, so the choice is the user's.

**What was left for Ernest.** The wording sent also had a session read the load before it reads a timing test's failure as a finding. That is a rule of the tests and not of the agents: a session runs its tests itself, and one that starts no agent never reads this page. It belongs in `CLAUDE.md`'s *Tests*, beside the rule that a flake is tested under what it was seen under. That file is cut from Ernest's, so Ernest words it first and the template takes it whole.

## A timing test under another session's load, 2026-11-17

`CLAUDE.md`'s *Tests* says that a timing test which fails under another session's load is run again on a quiet machine and not hunted, taken whole from Ernest's `CLAUDE.md`, which worded it first at the template's asking, and the template is tagged `v0.10.16` (Ernest's log, *A Load Another Session Makes*).

**The rule.** When a test that asserts a time, or a ratio of times, fails, the session reads the machine's load. Where another session made the load, the failure is said to the user with the load, and the test runs again on a quiet machine. Where it passes there, a log line naming the test and the load closes it, and no hunt follows.

**Why.** The sentence of `v0.10.15` has a session read the load before it starts an agent, and said nothing of the test that fails under a load already there. Such a failure was neither no finding nor a flake to hunt. A test that asserts a time fails under several times the machine's threads by scheduling alone, which says nothing of the program. No target can make another session's load again, so a hunt under what the failure was seen under cannot be run. In Ernest a timing test failed once under a load of 69 on 24 threads that two other repositories' sessions made, and passed in the next full run on a quiet machine.

**Narrow by design.** Any other test that fails under that load shows a race, so it is a flake, and the flake's rules keep it.

## A long run's first step is checked alone, 2026-11-17

`CLAUDE.md`'s *Tests* says that a step a long run rests on is checked in a call of its own before the run starts, taken whole from Ernest's `CLAUDE.md`, where it has stood since 2026-11-06, and the template is tagged `v0.10.17` (Ernest's log, *The Browser Test's Flake*).

**The rule.** A step a long run rests on, a pull or a build, is checked in a call of its own before the run starts.

**Why.** In Ernest twenty green runs of a flake's hunt had tested old code, since a pull chained before them failed unseen. A long run's result says something only of what it ran, and a first step that fails inside a chain leaves the run standing on what was there before. *Done* already reads make's exit status in a call of its own before a commit, and this is the same reading at a run's start. A flake's hunt here is such a run, so the rule holds for an application as it does for Ernest.

**How it was found.** The template took the flake's rules from Ernest and not this one beside them. It was seen when Ernest's *Tests* was read for the sentence of `v0.10.16`, and the repositories keep the same rules.

## What a timing test is, 2026-11-17

`CLAUDE.md`'s rule on a timing test under another session's load says what a timing test is, which ernest-httpd's objection to the sentence of `v0.10.16` asked for, taken whole from Ernest's `CLAUDE.md`, and the template is tagged `v0.10.18` (Ernest's log, *A Load Another Session Makes*, its paragraph *What a timing test is, said the same evening*).

**The rule.** A timing test is one whose failing assertion compares a measured time, or a ratio of measured times. The failure's text is read first: a test whose wait ran out of its deadline is no timing test but a flake, whatever the load.

**Why.** The sentence of `v0.10.16` spoke of "a test that asserts a time, or a ratio of times", which did not say whether a test whose wait ran out of its deadline is one. In ernest-httpd `Sessions.startsAnew` failed the same day under another session's load of 54 to 261, at a `receive` that waited 5000 ms and gave up. It looked like a timing failure under load and was a defect: the tests' stand-in shell never told its session `Written`, so output that came in two reads was read once, and the load only made the terminal split the output. A probe made it fail at will on a quiet machine.

Read as a timing test, the rule would have run it again on a quiet machine, seen it pass and closed a real defect with a log line. The rule saves a hunt, and there it would have hidden a defect, which is the costly way to be wrong. Its last sentence meant such a test for the flakes, and nothing forced that reading on a session that looks at a timeout under a load of 200.

**The failing assertion.** A test may both wait and measure, so what decides is the assertion that failed, and the term is defined once before the rule uses it.

## A run of items, 2026-11-18

`CLAUDE.md`'s *Done* gains a rule: a session may take the plan's next items one after another where they stand alone, and stops at the first thing that needs the user. It is written here first, then in Ernest's `CLAUDE.md` and the copies, and the template is tagged `v0.10.19` (Ernest's log, *A Run of Items*).

**The rule.** Where the plan's next items stand alone, the session takes them one after another, an agent for each, and closes and commits each before the next starts. It stops at the first thing that needs the user, however small: a decision, a surprise, a departure from the brief, a check that fails. The session judges that from each diff and its check. Where nothing stops it, it stops after three items, and one report to the user covers the run.

**Why.** The stop after each item is there so that the user sees an item's choices before the next builds on them. Where the items stand alone nothing builds on them, and for a small item the stop was most of its cost. The stop is kept wherever there is something to see: a surprise the session would have decided alone stops the run too.

**Two forms set aside.** Several items in one agent: its brief and its report become several, a failure in the middle leaves the later items on a tree that is not clean, and items that stand alone share nothing an agent's context could carry. Agents side by side in one checkout: they share its build directory, and a check that reads the whole tree fails one agent on another's half-written file.

**What follows it.** `docs/agents.md` says that each item of a run has an agent of its own. *The repository*'s sentence on a session's length reads one item or one run of items, and the checklist's last line places the report at the run's end.

## An item read against the items left, 2026-11-19

`CLAUDE.md`'s *Before code* gains a rule: an item is read against the items left when it is written into the plan. It is written here first, then in Ernest's `CLAUDE.md` and the copies, and the template is tagged `v0.10.20` (Ernest's log, *The Plan Read for Build Order*, its paragraph *The rule*).

**The rule.** Before an item is written into the plan, moved or changed there, the plan is searched for each section, file and name the item names. Each item left that names the same is read beside it: whether one needs what the other shows, builds or decides, whether both write one sentence, and whether a condition one states of the other can still be met. The item's paragraph names each item it follows, with the reason.

**Why.** A plan orders its items left by kind, and nothing read a new item beside them. In Ernest's plan one item was built before the item whose result it needed, and a reading of the whole plan then found eight orders wrong. Each came from an item written in, moved or given a new paragraph. Each pair shared a name, so a search finds the candidates, and the reading is of a few paragraphs.

**A form set aside.** A reader over the whole plan before each milestone finds the same clashes, days after the item was written and at an agent's cost. It stays what the user asks for.

## A brief sorts its runs, 2026-11-19

`docs/agents.md`'s *The brief* gains a sentence: a brief sorts its agent's runs into those bound by the processor and those that only wait. It is written here first, then in Ernest's `docs/agents.md` and the copies, and the template is tagged `v0.10.21` (Ernest's log, *A Brief Sorts Its Runs*).

**The rule.** The brief sorts the agent's runs by that test and names each kind: a race's probe and a run whose time is measured are bound by the processor, and a run that only waits, a test that fails by running out its deadline among them, goes side by side.

**Why.** The rule before it was right, and left the sorting to the brief's writer. In Ernest two briefs for work on timing put every probe and every test one at a time. Twelve tests that failed only by running out a deadline of 30 seconds then ran one after another, twice, and the machine stood idle for about ten minutes of each build's hour. A run that hangs until its deadline hangs the same beside eleven others.

## The short rules, 2026-11-21

`CLAUDE.md` is cut again, from Ernest's short file, and `docs/agents.md` follows Ernest's. The template is tagged `v0.10.22` (Ernest's log, *The Short Rules Stay*).

**What it was.** The file was a cut of Ernest's long one, some 4,900 words. Each rule of the long file was written after a mistake, and most said how to think. A session that weighs that many follows the strictest reading of the ones it remembers: in Ernest one item took most of a day in probes for 62 lines of code.

**What it is.** About 1,500 words: what is the user's, who decides, what the user wants of the program, and how a result is reported. It keeps facts, and gates, a question asked once before work starts. It drops checks, what is done at every act. A mistake adds no rule to it.

**New in it.** Whether a first user meets an item is asked when the item is written and before it starts. A corner that only a built program meets is a line of `known_issues.md` under `docs/`, which a copy begins at its first line, and becomes an item when the user takes it up. What a reading shows to be deterministic is verified once, and only what is intermittent is run again. A question about what Ernest or the code does is the session's own, and no agent's.

**What a copy loses.** The rules on a session's length and effort, a flake's hunt, a timing test under load, a proposal's life and the search of the plan before an item is written. A session that needs one works without it, and the user says where it is missed.

**The pages that cite the file** name its new sections: `docs/agents.md`, `docs/full_review.md`, `docs/release.md`, `docs/README.md` and a comment of `tools/docs.ern`. `docs/agents.md` also says that an agent's report comes back as its answer, and that a question is no diagnosis.


## A long item's file, 2026-11-22

`tools/docs.ern` reported a list item's paragraph past the measure with an empty file name, `:<line>: N words …`, where a line at or before the item's indentation ended it: `counted` called `ended("", reading)`, and `readsItems` compared the lines alone. `counted` now takes the file, and the test compares the file beside the line. Ernest's hunt for a result that is never empty found it, reading the tool (Ernest's log, *A Result Never Empty, Counted*). The template is tagged `v0.10.24`.

## Packages, 2026-11-23

`package.conf` takes the place of the Makefile's floor and dependencies, as Ernest's report §11.9 has them, and the template is tagged `v0.11.0` (Ernest's log, *An Installed Program's Packages*; its plan's MVP 4.4, item 4).

**What went.** `ERN_VERSION`, `DEPS`, `LOAD_PATH`, `RUN_LOAD_PATH`, `DEP_DIRS`, the `version` target, and the loops that fetched and built each dependency. `package.conf`'s `ernest` is the least release, which `ern build` holds the running `ern` to in its own words; `make lib` runs `ern unpack` and then each Erlang application's own make; `ern build src` builds each package before the program. With the target went its line for no `ern` on `PATH`, which the shell now says.

**`lib` is the manifest's alone.** A program's own Erlang stands under `erl/`, each application's `ebin` and `priv` where its make built them, and `--libs-dir erl` names it; nothing is linked under `lib`. The launcher gives its root by `--package-dir` and loses its loop over `lib/*/build`.

**The archive is a package.** It carries `package.conf`, the program's Erlang at its top, every application's beams in one `ebin/` and the `priv/` of the application of the program's name beside it, and no link, so that `ern unpack` takes it. An installation is laid out the same way, and the launcher names its `ebin/` by `--load-path`. Another application's `priv/` is refused, by `release` and `install` alike before either removes or writes anything, since the host would not find it there. `make clean` keeps the archives and the links under `lib/`.

**An earlier `ern`.** From 0.11.0 on, `ern build` refuses a release earlier than `package.conf`'s and names both. An `ern` before 0.11.0 has no `unpack` and stops `make` at `make lib`, with `ern: no job unpack`, before anything reads `package.conf`. The README says so, and the Makefile checks no release itself: the check is `ern build`'s, and parsing `package.conf` in shell would be a second one, against the report's *one way, one job*.

**The checker** reads a paragraph as Ernest's words tool does: a heading, a table row or a tag after a list item that its indentation ended is no prose, `1a.` begins an item, and a paragraph is shown by its first 60 bytes, its last character whole (Ernest's log, *The Three Tools in Ernest*).

## The full review, 2026-11-23

The template's first full review read `d8b7ab4` with Ernest's 0.11.0 candidate: K, the cold reader, and D, the documents reader, on Fable 5.2 at high, and C, the code reader, on Opus 5.5 at xhigh. S had no part, since the template takes no input from another party. Of 118 findings, 97 were fixed, 6 of those with a part dropped; 15 were Ernest's and became 13 lines of `docs/language_feedback.md`; 6 were dropped. The sort and the readers' lists stand in `docs/findings.md` at `c9bc7c1`, and each commit names the findings it fixed.

**An installation builds.** A compiled module runs only under the build of `ern` that wrote it (§11.2), so an archive installed as it was compiled ran under no other. `make install` now depends on `all`, as Ernest's own does: under the same `ern` it compiles nothing, and under another it builds again from the sources the archive carries. It and `uninstall` refuse a `lib/<name>` under `PREFIX` that holds no installation, before anything is removed.

**The release refuses first.** A development build of `ern`, a tracked file not committed, a file under `src/` that git does not track, and another application's `priv/` are refused before `make test` and `make doc` run, so that a refusal costs nothing and an archive holds only what is committed. A package under `lib/` travels as §11.9 has one, and nothing else of it.

**Both forms of the pages.** `make doc` writes the module pages, CommonMark, and the manual pages, roff, with `ern doc --man`. A library's archive carries the first under `docs/modules/` and the second under `docs/man/man3/`, where `man -M` finds them; `docs/man/` had held CommonMark, which `man` does not read.

**The history check reads the project's forms.** It refused plain words, so that a program whose domain has milestones, plans or readers could not write its own code. A comment now names no milestone, step or item with its number, no finding by its name after the word "finding", neither the plan's file nor the findings', and no date; a log entry's title stays allowed. Paths are held to what git tracks, past ASCII too, each finding with its line, and the logs and the proposals are left out. Where git tracks nothing, the checker refuses rather than passing.

**`docs/build.md`.** The Makefile, the launcher, the archive and the installation were stated only in `TEMPLATE.md` §4, which a copy removes, so a copy kept the code and lost its design. They move to `docs/build.md`, which a copy takes whole beside the Makefile below its variables, the launcher and `docs/release.md`. The README's steps now work in their order, from `git init` to the last `make test`, and each fact of the documents stands once, with its owner. The epigraph is the family's line, which every application begun from the template keeps.

**What waits.** Four changes to `CLAUDE.md`, the release of `ern` among them, wait for Ernest's session's reading and the user's word, as `docs/findings.md` gives them, and so do the messages to Ernest's session and to the copies. Nothing is pushed until Ernest's 0.11.0 is released.

**The round.** A cold reader over the README and a documents reader over the other documents the fixes changed read `d8b7ab4` to `7ceac48`, both on Fable 5.2 at high. Their 47 findings came to 28 lines: 21 fixed, 2 dropped, 4 lines of `docs/language_feedback.md`, and one sentence of `CLAUDE.md` that waits with the rest. The worst were the review's own: a copy kept the template's findings and feedback, step 6 promised a failure `make test` does not give, `make release` carried files git did not track, and an install cut short blocked the next one and `uninstall`.

**A package's modules stand under its name** because a dependent's `ern build` refuses any other (§11.9), and the package's own build holds no such rule. `docs/build.md` states the rule, and Ernest is asked for the check, rather than the Makefile writing a second one. A release's note is now held by the checker to name no log entry and no document reader, as `docs/release.md` and the README say.

## The library's renames, 2026-11-25

Ernest's 0.11.0 renames names and answers of its library in its MVP 4.4's full review (Ernest's log, *The Renames of the Library's Names*). The template meets one: `List.span` is `List.splitWhile`, which `tools/docs.ern` calls at eight places, and an `ern` built from `0a0a14ea` refuses the old name. The calls take the new name, so an earlier candidate of 0.11.0 no longer builds the template. The others, the swap of `Peer.compute` and `Peer.computeAt` and the seed first in `Random`'s answers among them, touch nothing here.

## The log split by day, 2026-11-26

A copy's log that nears 256 KB is split by day under `docs/log/`, in Ernest's form, and `tools/docs.ern` holds both forms; `TEMPLATE.md` §3 states the form. It is the template's issue 1, designed on 2026-11-13 and left unbuilt, since a check for a form no repository held met no need (principle 5). It is built now that ernest-httpd's log has passed 200 KB, the size the issue waited for: 205,415 bytes, 136 entries over 23 days.

**What changed from the issue.** `CLAUDE.md`'s *Writing* no longer holds the 250 KB rule, cut with the short rules on 2026-11-21, and it is not brought back: the checker refuses a log past the ceiling and says to split it, and a copy keeps the checker. `CLAUDE.md` changes only its owner row, which loses its link, since the link would name nothing in a split copy; the row waits with the other changes to `CLAUDE.md` in `docs/findings.md`. The checker now leaves a log's files out in two places, the paths and the paragraphs, and a release's note that names a log entry by a file under `log/` is refused, as one naming `log.md` is.

**The date** is the one an entry's first paragraph opens with, `*2026-10-30.*` or `*2026-10-13, decided 2026-10-26.*`, not its heading's as in Ernest's log. Every entry of both copies opens so, and three of httpd's stand out of their date's order and go to their day's file.

**No tool splits.** A copy splits once, by hand, and its `make test` holds the result. ernest-epx and ernest-httpd take the checker with the rest of `tools/docs.ern` from the final tag.

## Ernest agrees, 2026-11-27

The first step of the lock step after the full review. Ernest's session read what waited for it in `docs/findings.md` at `54f1eec`, against its own repository and both copies. It agreed with nine items, with four in other words, and objected in part to two (Ernest's log, *The Lines Go by the Tracker*). The user took every recommendation. `CLAUDE.md` gains the seven changes that waited, in Ernest's words where it gave them.

**The release of `ern`.** "A candidate Ernest's session names" would be false in a stranger's copy, which takes the file whole, so the archive is "a release or a candidate for one". A commit waits until its release is published, not only made, since whoever clones it can install only what is published.

**The files a copy takes whole.** They are not the same everywhere today. ernest-epx's `docs/release.md` has a step of its own, the window tried by hand, and ernest-httpd's Makefile has two targets of its own, so the sentence excepts what a copy added. The launcher is not named yet: ernest-httpd's differs in what it does, and its session says at the next step which difference is the template's. Ernest's `docs/clean_room.md` now points at the sentence, which is the list's one owner.

**The lines go by the tracker.** A line of `docs/language_feedback.md` goes to Ernest as an issue, by the Feedback form Ernest's tracker gained for it. The session files it, and the issue holds the line whole, its program in it. Principle 2 decides one route for each kind, and principle 3 a public issue with a number, where a message is seen by two sessions alone. A line of ernest-httpd's fell between two messages on 2026-11-26 and had no answer until the user asked. A security hole never goes as an issue. The seventeen lines carried by message close by message.

**A copy's upstream is the template**, so `CLAUDE.md` names one route for a rule, the template's tracker, which gains `rule.yml` beside the defect's form. The message between the template's session and Ernest's is the template's own, and stands in its design note's §5, with the rule that one of Ernest's comes whole but for what that section changes or drops.

**`template/`.** `TEMPLATE.md` and `TEMPLATE_LOG.md` move to `template/design.md` and `template/log.md`, so that the top level holds only what a copy keeps and the README's last step removes one directory. Where Ernest's log, the copies' or this one cites the old names, the citation is history and stays. `docs/agents.md` no longer says a review's documents are read at the session's own effort, which stopped being true when the two efforts parted; Ernest's page drops it too.

## The launcher and the run, 2026-11-27

ernest-httpd's session said which of its launcher's differences are the template's, and the user took them. `realpath`, of POSIX.1-2024, follows the launcher's links in one call where a loop over `readlink` took eight lines, with the same result (principle 2). An `ern` that cannot be found or is not an executable file is refused before the run, with status 127, where the shell had named a line of a script the operator did not write (principle 1); httpd's cold reader met it as a first user. The promise is that narrow: an `ern` that is executable and fails to start still gets the shell's words. The template's line for a bare `--config-dir` stands, since a launcher every copy takes cannot know the program's usage. With these, `CLAUDE.md` names the launcher among the files a copy takes whole.

**The run.** ernest-httpd's `make run` serves its example site, with a configuration and two steps before it, where the template's runs the launcher with no argument, which that program refuses. `run` now takes its arguments from `RUN_ARGS` and first builds what `RUN_NEEDS` names, both among the variables a copy edits and empty by default, so that the Makefile below them stays one file. `EXAMPLES_MADE` moves among those variables too, since httpd's names two directories, and the documents an unpacked archive carries leave out each it names.

**The forms.** A line may be a defect, and Ernest's tracker has a form for one, so *The work* files a line by the form that fits it, Defect or Feedback, as Ernest's `docs/clean_room.md` has it.

## The index a paragraph a day, 2026-11-27

The split log's index holds a paragraph a day, the days a blank line apart, and `tools/docs.ern` refuses two days with none between them. GitHub joins lines with no blank line between into one paragraph, so "a line a day" rendered as one run of links, where a reader of the index looks for a day (principle 1). Ernest's own index stands so, all 71 of its days, and the template's form, cut from it, had said a line; ernest-httpd's split set its days apart and showed the difference. One form is stated and held (principle 2).

## Ernest's answers to the seventeen lines, 2026-11-27

Ernest's session answered each line of `docs/language_feedback.md` on 2026-11-26 (Ernest's log, *The Applications' Lines Sorted*, its *Decided* and *Built*), and each answer was checked against the released 0.11.0. Ten are in it, and their lines go: `ern doc` refuses a module `index` (KE1), `--doc-root` (KE2), `List.findIndex` (KE3), `CHANGES.md` opening with 0.11.0 (KE6, C49, DE1), `priv` beside `ebin` in §11.2 (DE2), the deployment guide's build by the running `ern` and its configuration directory kept out of a repository (DE3, DE4), guide §7.1's lookup (K16), ``help: write `Path(...)` `` (K17), and `ern test` over a directory as §11.2 states it (C48). Two stay, held by Ernest's plan: `Markdown`'s lines (C47), Ernest's 320, and a near name (K18), Ernest's 289.

**The five not taken go, agreed.** `--check`'s bare paths serve a tool, and make's echo names the command (KE4). A let's body now begins the next line, which took the deep column away (KE5). The guide's links to the repository at the tag stay put (KE7). The prefix `Ernest.` keeps a library's pages apart from the system's (SE1). A package held to its namespace in its own build is the template's check, not `ern`'s (K15): `make test` builds a small dependent in a scratch directory, so that a library that breaks each dependent does not pass its own tests (principle 3). This reverses *The full review*'s round, which asked Ernest for the check; with none in `ern`, the template's is no second one.

## The pages by their roots, the stage and a dependent, 2026-11-27

Three of Ernest's answers became the template's code. `make doc` writes the module pages under `build/doc/` and the manual pages under `build/man/` by `--doc-root` (KE2), so that the release copies two directories where a `find` over the build root passed over every path with a `-` to miss its own staging. The release stages its archive's tree in `stage/`, outside every build root, so that one cut short leaves no copy of `build/` for `ern test build` to run again (C48). `make test` builds a dependent of the program in a temporary directory, so that a module outside `src/<name>.ern` and `src/<name>/` fails the program's own tests with `ern`'s words, where it had passed until someone else's build (K15, principle 3).

**The dependent's packages.** It names each package of the checkout's `lib/` beside the program, by its directory and its `VERSION`, since §11.9 has a root manifest name every package its packages name, and a copy's first package would otherwise fail its tests for nothing in its code; `lib/` is read where `package.conf` would need a JSON reader in the Makefile.

`tools/docs.ern` finds the index's heading by `List.findIndex` (KE3), the function it had written for itself.

## A reader follows its brief instead, 2026-11-27

`docs/agents.md` had a review's reader's brief carry two rules of `CLAUDE.md`, untracked files and the style guide, where `docs/full_review.md` has it keep one; ernest-httpd filed it as the template's issue #4. The two sentences now give every agent's brief its two lines and make a reader the exception, its brief standing in place of `CLAUDE.md`, so that `full_review.md` alone says what a reader keeps. Ernest's page took the same fix (Ernest's log, *A Reader Follows Its Brief Instead*).

## A code span by its run, a fence by its length, 2026-11-27

`tools/docs.ern` split a document's text at every backtick, so a double-backtick span holding a backtick, as ernest-httpd's design writes a token's characters, swapped prose and code to the end of the file: every path after it went unchecked, and `make test` passed. A fence closed at any line of three backticks or tildes, so a block of four that quoted a line of three ended there, as did a block of backticks at a line of tildes. ernest-httpd filed it as the template's issue #3. Ernest's 320, which has the checker read by `Markdown.parse`, waits for Ernest's MVP 4.5, so the defect is fixed now (principle 1: the checker reads a document as its reader sees it).

The two rules are the library's, in its words, so that the checker and the library agree where 320 replaces the one with the other: a code span closes at a run of exactly as many backticks, a line break in it is a space, and one space at each end is dropped when both are there and the span is not all spaces; a fenced block runs to a closing fence of its character at least as long as the opening one, or to the end of the document. A span does not cross a blank line, since the checker reads no block that would end it, and a run that no run closes is text.

Ernest's session agreed, and kept it to the two rules: reading spans by `Markdown.parse` would give one document two readers, which can disagree about what is fenced. The known issue narrows to what the checker still reads by its own rules.

## What of `priv/` an archive carries, 2026-11-27

`release` and `install` copied the whole `priv/` of the application of the program's name. So ernest-epx's archive carried 110 entries where its program loads `epx_nif.so` alone, among them eight of Microsoft's core fonts, which no one may pass on. ernest-epx filed it as the template's issue #5, and its 0.3.0 waited on it. Ernest's report says where the host finds a `priv/` and nothing of what it holds, so the fix is the template's. `ERL_PRIV`, among the variables an application edits, names what of that `priv/` the archive carries, and nothing else of it goes, so that a file new to `priv/` ships only once it is named (principle 3, and the taste for lean). A copy that needs the whole writes `.`.

An empty `ERL_PRIV` was first to carry the whole, as before. Ernest's session read that as two meanings for one variable, and as the defect kept for the next application that names nothing, and the user took its change: an empty one is refused where there is a `priv/`, as are a path that leaves `priv/` and one the build did not make. The paths are read once `test` has built `erl/`, since a NIF stands only then. An unpacked archive's `priv/` is already narrowed and is carried as it stands. A list of what to leave out was weighed and not taken, since it ships a new file unless someone remembers to name it.

## The tops a copy may have, 2026-11-27

`tools/docs.ern` checked a backticked path only under a directory the repository tracks. So a file a copy takes whole could name a path under `examples/`, `deploy/`, `erl/` or `test/` that the template's `make test` never checked and a copy's refused, as `examples/build` was. ernest-epx filed it as the template's issue #6. The four are tops now in every document of every repository, beside the tracked ones, as `template/design.md` §3 names them for a copy: a path under one that names nothing names nothing wherever it stands, and a copy that has the directory checked it already (principle 3). `lib/`, which the build fills, stays out. `docs/full_review.md` names the README under `deploy/` in words, since its path names nothing here.

Checking only the files a copy takes whole with the four added was weighed and not taken, since the checker would hold a second list of what `CLAUDE.md` owns. Ernest's session agreed, and noted the mirror: a path the template has and a copy lacks passes here and is refused at the copy's first `make test`, loudly. It is a line of the known issues, and no file a copy takes whole names one.

## The Rule form names where a rule was found, 2026-11-27

On the user's word, what Ernest's session finds wrong in the template or asks of it comes as an issue on the template's tracker, and a message between the two sessions carries news alone (Ernest's `docs/clean_room.md`). The Rule form said a copy found the rule and asked for "The copy", which left Ernest's session out; it filed that as the template's issue #7, with the wording. The form now asks where the rule was found, a copy's repository or Ernest's, and what happened there, in Ernest's words. `template/design.md` §3 says the form brings a rule from a copy or from Ernest's session, and §5 that what Ernest's session asks of the template comes by an issue, the other way staying by message (principle 1: a form that misnames who fills it asks for a wrong answer).

## What a copy keeps of the known issues, 2026-11-27

ernest-epx took v0.11.1 and asked two things of `docs/known_issues.md`. The checker's Markdown line ended at "a line of `language_feedback.md`", which a copy does not hold, so it now ends at Ernest's feedback 320, in epx's words, and reads true wherever the checker goes. The line on the template's own `make test` is no checker's: `template/design.md` §3 now says the file holds the checker's lines, which a copy keeps, and the template's own, which a copy removes, and the README's step 6 lists them among what a copy removes.

## The icon is Ernest's site's, 2026-11-28

`assets/README.md` and `template/design.md` §3 called `icon.png` the repository's icon, which GitHub never shows: a repository shows its owner's avatar, and takes only its social preview. ernest-epx had to ask what used it, and filed it as the template's issue #8. Ernest's site does, where it lists the projects written in Ernest: it holds a copy of each listed project's icon, a PNG of 128 by 128, made by hand when the project is listed, and reads nothing from the project's repository (Ernest's log, *Projects, a Page of Their Own*). The two sentences now say so, in the words of Ernest's session (principle 1: a file says what uses it). What else the site lists of a project, its name and its purpose, is Ernest's, and the README's opening already gives the purpose it is read against.

## An installation made before `package.conf`, 2026-11-28

`make install` and `make uninstall` took `lib/<name>` for an installation only where it was empty or held `package.conf`, which came with v0.11.0. Every install of the template's from v0.9.0 to v0.10.24 wrote none, so a copy's next release refused its own earlier installation, and only the old archive's `make uninstall` removed it; ernest-httpd's live server stands on one, and it filed the template's issue #9. Every one of those installs wrote `build/<name>.erc` under the tree, and today's does too, so that file is the third case the two targets take. A narrower promise, an older installation removed first by its own archive, was weighed and not taken, since an operator without that archive would remove paths by hand.

Ernest's session agreed, and found that the older tree, holding no `package.conf`, would break the promise that `lib/<name>` is an installation at every step: removed in no order, it could lose `build/<name>.erc` before the rest and leave a tree no case takes. So where the tree holds `build/<name>.erc` and no `package.conf`, both targets copy `package.conf` into it before anything there goes, and the existing order holds from there.
