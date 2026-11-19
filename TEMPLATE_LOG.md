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
