# Findings

The full review of commit `d8b7ab4`, read with `ern 0.11.0+93a13b13`, Ernest's candidate archive: K, the cold reader, and D, the documents reader, on Fable 5.2 at high, and C, the code reader, on Opus 5.5 at xhigh. S has no part, since the template takes no input from another party. A line per finding, each by its reader's letter and number. A finding of Ernest's is marked *Ernest's*, and K's and D's are numbered KE and DE, apart from their lists. Each reader's whole list stands below the lines.

K read the Makefile, the launcher, `src/name.ern`, `package.conf` and the issue forms, which its brief leaves out; its findings stand.

## Where each fix goes

A fix is carried as the file it touches is.

- **To the copies whole**, from the next tag: `tools/docs.ern` (K2, K11, C8, C9, C14 to C16, C18, C20 to C24, C26, C27, C29 to C31, C33 to C35, C37, C39 to C46, D12, and Q2 and Q3), `docs/full_review.md` (D3, D4, D5, D25's reading), `CLAUDE.md` (D7, D11, D16, D25's row, and Q5), and, by Q4, the Makefile but its variables, the launcher, `docs/release.md` and the new `docs/build.md`.
- **To Ernest's session first**, for its reading and the user's decision, since its file is upstream: each change to `CLAUDE.md` and `docs/agents.md`. These wait, as *Waiting for the user's word* says.
- **The parts the same everywhere**, taken whole by Q4: the Makefile below its variables (K3, K4, K6, K7, K9, K10, K12, K27, C1, C2, C12, C17, C19, C28, C38, Q1, Q6), the launcher (K5, K8), and `docs/release.md` (D5, D14). `.gitignore` (D2) stays a copy's own, and each copy is told of the line.
- **The template's own**, its README's steps and *Building*, `TEMPLATE.md`, `src/name.ern`, and the starters `docs/README.md`, `docs/design.md`, `docs/plan.md` and `CHANGES.md`: no copy takes them. Each copy is told where it has a sentence that a fix changed here, and decides for itself.
- **Ernest's lines** go to `docs/language_feedback.md`, which Ernest's session reads.

## Waiting for the user's word

Messages to Ernest's session wait until the user says so. What would go stands here, so that nothing is lost meanwhile.

**The changes to `CLAUDE.md`.** Ernest's session reads each against Ernest's `CLAUDE.md` and `docs/clean_room.md` and gives the user a recommendation. Each is then written only once the user decides it. Each is given here as it would read:

- **D7, the life of a feedback line.** *Where a fact lives*: "`language_feedback.md`, under `docs/` from its first line: what writing Ernest felt against the principles, a line each, as long as *The work* says." *The work*'s sentence, "A line the next release answers goes…", stays the owner. TEMPLATE.md §1 points at it, which is the template's own and is not waiting.
- **D11 with Q5, the release of `ern`.** *The work*: "**The program is Ernest, written for the release `package.conf` names**, the least it builds with; until 1.0 a later release may refuse it, until the program rises to that release. That `ern` is installed from an archive of Ernest's, a release or a candidate Ernest's session names, as a user installs it, and never from a checkout, and a commit that needs a release not yet made is pushed only after it is made."
- **Q4 with D16, the files a copy takes whole.** *What is the user's*: "This file, `docs/agents.md`, `docs/build.md`, `docs/full_review.md`, `docs/release.md`, `tools/docs.ern`, the Makefile and the launcher are the template's, `ernest-template`'s, and change there. A copy takes each again whole: this file but for its title and the sentence under it, the review but for the readers the copy added, the Makefile but for its variables, and the launcher under the program's name." TEMPLATE.md §8, `docs/full_review.md` and `docs/log.md`'s first entry point at it.
- **D25, a row of *Read when the job starts*.** "Building, testing, running | `README.md`'s *Building* and *Running*".

**What Ernest's session is told.** The 13 lines of `docs/language_feedback.md` are noted there, at `2cbb6d3`, and are sorted after Ernest's own third leg. Not yet told: Q4, that a copy now takes the Makefile, the launcher, `docs/release.md` and `docs/build.md` whole, which Ernest's own `CLAUDE.md` does not take.

## The sort

Each line ends in its verdict. **Fix** gives the fix's shape. **Drop** gives the reason. **Ernest** makes a line of `docs/language_feedback.md`. **Fix, by Qn** follows the user's decision n below. A line that repeats another names it.

The questions, each decided by the user:

- **Q1, decided: `install` depends on `all`.** K24, C10, D1, DE3: a compiled module runs only under the build of `ern` that wrote it. `install` depends on `all`, as Ernest's own does, so that another `ern` rebuilds the stale modules from the archive's source, and a checkout's stale `build/` is built again. TEMPLATE.md §4 says that the compiled modules serve an operator of the same release, and *Running* that an installed program is installed again from its archive after its `ern` changes.
- **Q2, decided: the project's own forms alone.** C7, K18: a bare word passes. The check refuses a milestone, step or item with its number, `Milestone 2` or `item 4`; a finding by its letter and number after the word "finding"; the name of the plan's or the findings' file; `the log's *…*`; and a date in a comment. The README names those kinds.
- **Q3, decided: the indented table row now, the rest for Ernest.** C13: the checker tests a table row on its trimmed line. The lone backtick and the longer fence wait for `Markdown.parse` with lines, C47, whose line in `language_feedback.md` names them; the checker then reads by it, and its own reading goes.
- **Q4, decided: a copy takes them whole, and they gain a document.** D16, D21: `CLAUDE.md`'s *What is the user's* names every file a copy takes whole from the tag: the four it names, with their exceptions; the Makefile but its variables; the launcher, under the program's name; and `docs/release.md`. TEMPLATE.md §4 moves to `docs/build.md`, which a copy keeps and takes whole. TEMPLATE.md §8, `docs/full_review.md` and `docs/log.md`'s first entry point at the list. `.gitignore` and the issue forms stay a copy's own, and each copy is told what changed in them.
- **Q5, decided: a release or a named candidate.** D26: `CLAUDE.md`'s sentence reads that the `ern` is installed from an archive of Ernest's, a release or a candidate Ernest's session names, as a user installs it, and never from a checkout; a commit that needs an unreleased `ern` is pushed only after that release. TEMPLATE.md §4 keeps a development build passing. Agreed with Ernest's session first.
- **Q6, decided: both forms in a library's archive.** K25, D23: `make doc` runs `ern doc src` and `ern doc --man src`. A library's archive carries the roff pages under `docs/man/man3/`, where `man -M` finds them, and the CommonMark under `docs/modules/`, its index as the README. The documents call the CommonMark "the module pages" and the roff "the manual pages". An application's `install` puts no manual page, as before.
- **Q7, decided: the family's line.** D22: every application begun from the template keeps the epigraph, and TEMPLATE.md §3 says so in a sentence.
- **Q8, decided: the texts as they stand.**
  - K2: `docs: git tracks no file here; git add the repository's files first`
  - K6, C3: `a release is made from committed files alone, and these are not:`, and the files, a line each
  - K8, C6: `<name>: --config-dir takes a directory: <name> --config-dir dir [argument]...`
  - K10, C19: `a release is not made with a development build of ern, and this is ern <version>`
  - K12: `make test runs in a checkout of <name>, and this directory has no tools/`
  - C1: `<PREFIX>/lib/<name> is there already and holds no installation of <name>`, and for `uninstall` `<PREFIX>/lib/<name> holds no installation of <name>`

### K, the cold reader

- K1: README step 2's `make test` cannot pass before steps 3 and 6. **Fix**. Step 2 says that the template's own lines fail until steps 3 and 6, and `make test` closes step 6.
- K2: a clone with `.git` removed fails `make test`; after `git init` with nothing staged the documents' check reads nothing and passes. **Fix**. A copy that is a clone without `.git` begins with `git init` and `git add -A`. The checker refuses where git tracks no file (Q8).
- K3: in an unpacked archive with an Erlang application, `make`, `make run` and `make doc` stop at `erl/<app> is empty`. **Fix**, with C4. `lib`'s loop over `ERL_DEPS` runs only where `erl/` stands.
- K4: `make -j` fails from a clean tree that names a package; nothing orders `build` after `lib`. **Fix**, with C5. `build: lib`.
- K5: an installed launcher reached through a symbolic link does not find the program. **Fix**, with C11. The launcher resolves its own path through links, and runs `cd` with `CDPATH` empty.
- K6: `make release` ships the compiled form and the page of an untracked module. **Fix**, with C3 and C38's two copies. In a checkout, `release` refuses a changed tracked file and an untracked file under `src/` (Q8), and copies the `.erc` one way.
- K7: a library module named `index` loses its page, and `docs/man/README.md` links to it. **Fix**. The listing is left out by its path, `./index.md`.
- K8: `bin/<name> --config-dir` with no directory answers in the shell's words. **Fix**, with C6. The launcher refuses `--config-dir` without a value (Q8). An empty value goes to `ern`, which refuses it.
- K9: `make clean` leaves what `make lib` built under `erl/`. **Fix**, with C17 and D10. The README and the Makefile say that `make clean` leaves what each Erlang application built. `clean` removes `lib/<name>` only where `lib/<name>-*.tar.gz` stands beside it.
- K10: `make release` refuses a build of `ern` that is no release only after tests and pages; the README does not say it refuses one. **Fix**, with C19. The release check runs before `test` and names the version it found (Q8). The README's `make release` line says "with a release of `ern`".
- K11: the checker reports one comment under `src/` twice. **Fix**. A module's comment line is read once.
- K12: `make test` in an unpacked archive fails with `ern format: tools: no such file`. **Fix**. `make test` refuses where there is no `tools/` (Q8).
- K13: `<name>` stays in a finished README; a library keeps *Running* and the `make run` and `make install` lines. **Fix**. Step 1 replaces `NAME` and `<name>`, and says what a library removes: *Running*, and the `make run` and `make install` lines.
- K14: nothing in a copy's tree says which tag of the template it was begun from. **Fix**. Step 3 says where the tag is read: the template's newest tag on its GitHub page.
- K15: the README does not say what an example is given. **Fix**. A sentence on what an example is given and must write.
- K16: the README does not say what a module under `test/` holds or where it runs. **Fix**. A sentence on `test/`: modules of tests that run the program, the checkout their working directory.
- K17: the README does not give the form of a design citation. **Fix**. Step 2 gives the form `// design §n: …` above a test, and the rule that every section is cited.
- K18: the README does not say what "names the project's history" refuses. **Fix**, by Q2.
- K19: the build's needs beyond `ern` are not listed: git, `cpio`, `sha256sum`. **Fix**. The README names git, `cpio` and `sha256sum`. **Drop** macOS: Ernest is tested on Linux.
- K20: *Running* does not say the launcher needs `ern` on `PATH` or `ERN`. **Fix**. *Running* says that the launcher runs the `ern` on `PATH`, or `ERN`.
- K21: `make run` passes the program no argument. **Fix**. The `make run` line says that arguments go through `bin/<name>`.
- K22: no step says `src/name.ern` goes. **Fix**, with D22. Step 1 renames `src/name.ern` beside `bin/name`.
- K23: another application's `priv/` is refused only at install and release, and the remedy is unexplained. **Fix**. Step 4 says that only the application of the program's name may carry `priv/`, and another is a package of its own.
- K24: an unpacked release runs only under the build of `ern` that compiled it (not run). **Fix**, by Q1.
- K25: `docs/man/` holds CommonMark, which `man` does not read. **Fix**, by Q6.
- K26: `LICENSE` keeps the template author's copyright line. **Fix**. Step 4 says "with its year and holder".
- K27: small matters: the epigraph and "the line under the title", `make examples` with no example, `ACKNOWLEDGMENTS.md` not shipped, the pictures in every archive, stray spaces in two echoed commands. **Fix** the step 6 wording, which means line 5, and the epigraph by Q7. **Fix** `ACKNOWLEDGMENTS.md`, which `DOCS` takes beside `THIRD_PARTY_LICENSES`. **Fix** the stray spaces by `$(strip …)`. **Drop** `make examples` with no example, since its message says why. **Drop** the pictures in the archive, since a copy's README may show its own.
- KE1, *Ernest's*: `ern doc src` overwrites the page of a root module named `index` with its listing, in silence. **Ernest**. `ern doc` overwrites a root module `index`'s page with the listing, in silence.
- KE2, *Ernest's*: `ern doc` has no place for the pages apart from the `.erc`. **Ernest**. `ern doc` has no root for the pages apart from the `.erc`; K7 fixes the template's own sifting meanwhile.
- KE3, *Ernest's*: the library has no `List.findIndex`. **Ernest**. No `List.findIndex`.
- KE4, *Ernest's*: `ern format --check` answers with a bare path. **Ernest**. `ern format --check` says a bare path, not what is wrong.
- KE5, *Ernest's*: `ern format` hangs a long call's arguments under its bracket. **Ernest**. `ern format` hangs a long call's arguments under its bracket, which a test of one expression cannot avoid.
- KE6, *Ernest's*: the installation's version text is `0.11.0+93a13b13`, no release. **Ernest**, with C49 and DE1, as one line. The candidate's `CHANGES.md` stops at 0.10.0, though its README is headed 0.11.0. The version text itself is a candidate's, and no finding.
- KE7, *Ernest's*: the guide points outside the installation for a module's documentation. **Ernest**. Guide §7.1 sends the reader outside the installation, to a page of the repository.
- KE8, *Ernest's*: forms repeated in the Ernest K wrote, with counts. **Drop**. The reader makes no ask, and the counts are mild.
- KE9, *Ernest's*: messages that needed no guessing (no ask). **Drop**. No ask.

### C, the code reader

- C1: `install` and `uninstall` take any directory at `PREFIX/lib/NAME` for the program's and remove it, and `share/doc/NAME` unchecked. **Fix**. `install` and `uninstall` refuse a `PREFIX/lib/NAME` that holds no `package.conf` and `build/NAME.erc`, before anything is removed (Q8), and remove `share/doc/NAME` only then.
- C2: a package under `lib/` that is a link is copied whole into the archive and the installation, `.git/` and `.env` among it. **Fix**. A package under `lib/` is copied as §11.9 has one: `package.conf`, `VERSION`, `src/`, `build/`, `ebin/` and `priv/`.
- C3: `make release` packs an uncommitted working tree. **Fix**, with K6.
- C4: the `lib` loop stops `make` and `make run` in an unpacked archive with no `erl/`. **Fix**, with K3.
- C5: `all: lib build` lets `make -j` build before anything is unpacked. **Fix**, with K4.
- C6: the launcher's `--config-dir` with an empty or missing value runs silently not as a node, or fails in the shell's words. **Fix**, with K8.
- C7: the history check refuses plain English words, so a program whose domain has milestones, plans or dates cannot write its own code. **Fix**, by Q2.
- C8: the path check reads the log and the proposals, which name paths that are gone or not yet written. **Fix**. The path check leaves out the log and the proposals, as the measure does.
- C9: an Ernest block of the README that quotes a comment line is refused. **Fix**. A part is held against the module as written as well as without its comments.
- C10: `install` builds nothing, so an installed archive runs only under the `ern` build that made it, and a checkout's stale `build/` installs. **Fix**, by Q1.
- C11: the launcher's root is wrong through a link of its own name, or with `CDPATH` set. **Fix**, with K5.
- C12: `|| true` in `release` hides a failed copy of the launcher. **Fix**. `if … then … fi` for the launcher's copy.
- C13: the checker's own Markdown reading fails on a lone backtick, a longer fence and an indented table row. **Fix**, by Q3, the indented table row; the rest with C47.
- C14: the path check holds a path to the working tree, not to what git tracks. **Fix**. A path under a tracked top is held to `git ls-files`.
- C15: the checker cannot read a tracked name past ASCII. **Fix**. `git -c core.quotePath=false ls-files -z`, split at NUL.
- C16: "docs: not UTF-8" names no file. **Fix**. The message names the file, `docs: <file>: not UTF-8`.
- C17: `make clean` leaves `erl/`'s build and removes any directory under `lib/`. **Fix**, with K9.
- C18: an `export let` test is no test to the checker. **Fix**. A leading `export ` is taken off before `let`.
- C19: `release` refuses a development `ern` only after `test` and `doc`. **Fix**, with K10.
- C20: `findsPaths` passes with the wildcard, metavariable and space rules removed. **Fix**. Each test gains the case that its finding shows passing broken.
- C21: `findsCitations` passes with `listed`'s comma and next-line rules broken. **Fix**. Each test gains the case that its finding shows passing broken.
- C22: `findsTested` passes with the blank-line rule broken. **Fix**. Each test gains the case that its finding shows passing broken.
- C23: `findsHistory` and `findsNotes` pass with any one refused form removed. **Fix**. Each test gains the case that its finding shows passing broken.
- C24: `readsItems` passes with the item's indentation rule removed. **Fix**. Each test gains the case that its finding shows passing broken.
- C25: `src/name.ern`'s test passes whatever the module does. **Fix**. The placeholder's test captures `main`'s output, so that it fails once `main` is written.
- C26: `tools/docs.ern` cites CLAUDE.md's *Writing* for two rules it does not state. **Fix**, with D12. The two citations of *Writing* go.
- C27: the checker's comment on two spaces before `#` does not say what the code does. **Fix**. The comment says what the code holds.
- C28: three Makefile comments no longer hold. **Fix**. The three comments say what the code does.
- C29: the checker's header leaves out code it runs. **Fix**. The header states the code it runs.
- C30: 22 sites of `… == false` where Ernest has `!`. **Fix**. `!` for `== false`.
- C31: each check reads the documents again, and the reading is spread over ten functions named as nouns. **Fix** the names, each function that does something named as a verb. **Drop** the single reading: it changes nothing a user sees, and it would be a rewrite.
- C32: four fence trackers and three state records where one pass would do. **Drop**. One pass would be a rewrite, and Q3 may replace the reading.
- C33: `notice` repeats 150, and 5000 stands bare at four sites. **Fix**. `notice` takes `measure`, and one named bound replaces the four 5000s.
- C34: `isChecked` and `numbered` stand under another banner than their users'. **Fix**. Each function moves to its user.
- C35: slices by `String.size` where `stripSuffix` and `stripPrefix` would do, and two one-clause matches. **Fix**. `stripSuffix`, `stripPrefix`, the `"make" :: _` pattern and the two one-clause matches.
- C36: sentinels where `Optional` would say "nothing begun". **Drop**. `Optional` in place of the sentinels would change three state records for no gain a user sees.
- C37: "names nothing" is the one finding with no line number. **Fix**. "names nothing" gives the line, since a user looks for it.
- C38: three Makefile forms: a `foreach` over one value, two ways to copy the `.erc`, an eight-line sentence. **Fix**. The `foreach` over one value goes, the two copies of the `.erc` are one (K6), and the eight-line sentence is split.
- C39: the checker's tests carry `///`, the form its own rule says carries no citation. **Fix**. The tests' comments use `//`.
- C40: `quoted` and `commands` answer the opposite of their names. **Fix**. Each name says what its value or its work is.
- C41: `read` names three things. **Fix**. Each name says what its value or its work is.
- C42: `sectionsIn` answers a note's lines; rename it. **Fix**. Each name says what its value or its work is.
- C43: `isNumber` asks only whether a word begins with a digit. **Fix**. Each name says what its value or its work is.
- C44: `isMeasured` also chooses the commands' files, and `isChecked` does not say what is checked. **Fix**. Each name says what its value or its work is.
- C45: `line` is both a line's text and its number, and a number has three names. **Fix**. Each name says what its value or its work is.
- C46: five names that do not say what they are. **Fix**. Each name says what its value or its work is.
- C47, *Ernest's*: `Markdown.parse` gives no block a position, so a tool that names a line writes its own reader. **Ernest**. `Markdown.parse` gives no block a line, and meanwhile the checker misses a lone backtick and a longer fence (C13).
- C48, *Ernest's*: `ern test` runs a `.erc` under a directory that `ern build` would refuse. **Ernest**. `ern test` runs a `.erc` under a path that `ern build` refuses.
- C49, *Ernest's*: the installation prints `ern 0.11.0+93a13b13`, no release. **Ernest**, with KE6.
- C50, *Ernest's*: forms repeated: a time on every local `Fs` call, and `index + 1` at five sites (no ask). **Drop**. The reader makes no ask.

### D, the documents reader

- D1: TEMPLATE.md §4 says the compiled modules run "under any release of its floor"; report §11.2 refuses another build's. **Fix**, by Q1.
- D2: `.ernest/` is not a configuration directory, so `.gitignore` does not keep a node's key out. **Fix**. `.gitignore` ignores `private-key.pem` where `.ernest/` stood, and TEMPLATE.md drops "whose `.ernest/`". DE4 goes to Ernest.
- D3: `full_review.md` says a reader writes its list to a file; `agents.md` says an agent cannot. **Fix**. `full_review.md` says that a reader hands its list back as its answer, and the session keeps it.
- D4: `full_review.md` says "the `ern` the Makefile names"; `package.conf` names it. **Fix**. "an `ern` of the release `package.conf` names".
- D5: a fresh clone of a program that names a package stops at `make lib`; `full_review.md` and `release.md` do not say the archives come first. **Fix**. `full_review.md` and `release.md` put each archive `ern unpack` names under `lib/` between the clone and `make test`.
- D6: no document says a package's modules stand under its name, which §11.9 holds. **Fix**. Step 2 and TEMPLATE.md §3 say that the modules stand at `src/<name>.ern` and under `src/<name>/`.
- D7: three lifetimes for a line of `language_feedback.md`. **Fix**. *The work* in `CLAUDE.md` owns the life of a line, and *Where a fact lives* and TEMPLATE.md §1 point at it. Its `CLAUDE.md` part is agreed with Ernest's session first.
- D8: TEMPLATE.md §1 says an application has no Erlang of its own and no section numbers to cite. **Fix**. Both phrases go.
- D9: TEMPLATE.md §2 cites §8.4 and §11.2 for `priv/`, which they do not state. **Fix**. TEMPLATE.md §2 cites §11.9 for a named package's `priv/`, and calls the rest the host's rule. DE2 goes to Ernest.
- D10: README and Makefile say `make clean` removes what `make lib` wrote; `erl/`'s build stays. **Fix**, with K9.
- D11: CLAUDE.md and the README promise later releases; TEMPLATE.md gives the reason they cannot. **Fix**. One sentence: `package.conf` names the least release, and a later release may refuse the program until it rises. Its `CLAUDE.md` part is agreed with Ernest's session first.
- D12: `tools/docs.ern` cites CLAUDE.md's *Writing* for two rules it does not state. **Fix**, with C26.
- D13: the release's steps are listed in TEMPLATE.md §6 and `release.md`, and differ. **Fix**. TEMPLATE.md §6 points at `release.md`.
- D14: the note's contents are stated three times. **Fix**. `release.md` owns the note's contents and says that the note is written from the design's diff. `CHANGES.md` and TEMPLATE.md point at it.
- D15: `ern 0.11.0` is written in the README and the issue form beside `package.conf`. **Fix**. The README says "the release `package.conf` names" without its number. **Drop** the issue form, whose placeholder is an example.
- D16: the template's four files are listed four times, and nothing says how a copy takes a change to the rest that is "the same everywhere". **Fix**, by Q4.
- D17: the catalogue of documents lives in three places, and `docs/README.md` omits four. **Fix**. `docs/README.md` names `SECURITY.md` and `assets/README.md`. **Drop** the rest, since *Where a fact lives* names owners and not the catalogue.
- D18: the targets are listed three times and differ; "eleven targets". **Fix**. TEMPLATE.md names no count, and the README's lines and the Makefile's comment agree on what `make test` holds.
- D19: TEMPLATE.md's *The floor* uses the report's word for another thing. **Fix**. The paragraph is headed *The least release*.
- D20: `deploy/` is named four times and defined nowhere. **Fix**. TEMPLATE.md §3's *What appears when needed* names `deploy/`, what an operator reads.
- D21: the launcher, the archive and the installation are stated only in TEMPLATE.md §4, which a copy removes. **Fix**, by Q4.
- D22: the placeholder says to rename `src/name.ern`, which no step says; the epigraph is unexplained. **Fix**, with K22. **Fix** the epigraph by Q7.
- D23: "manual pages" for what `make doc` writes, which are CommonMark. **Fix**, by Q6.
- D24: TEMPLATE.md §5 says the design is not cited by number from outside, yet the note and the issue form cite it. **Fix**. TEMPLATE.md §5's reason goes, which the note and the issue form contradict.
- D25: smaller: CLAUDE.md's *Building* row covers *Running*, "the stronger model", pictures no document shows, "its types", "all the code", the plan's restated rule. **Fix** *Read when the job starts*'s row, to *Building* and *Running*, which is the template's own row. **Fix** the pictures' wording, "which the documents may show". **Fix** C's reading in `full_review.md`, which gains `package.conf`, `.gitignore` and `.github/`. **Fix** `plan.md`'s restated rule, which points at `CLAUDE.md`. **Drop** "the stronger model", since the names are the memory's by design. **Drop** "its types", what a copy's design adds.
- D26: CLAUDE.md's release archive beside TEMPLATE.md's "unreleased builds". **Fix**, by Q5.
- DE1, *Ernest's*: the installation is no release, and its `CHANGES.md` stops at 0.10.0. **Ernest**, with KE6.
- DE2, *Ernest's*: the report is silent on `priv` outside a named package. **Ernest**. The report says nothing of `priv` under `--libs-dir` or an `ebin` that `--load-path` names.
- DE3, *Ernest's*: no way to carry a runnable program to another build of `ern`. **Ernest**. A compiled program cannot be carried to another build of `ern`; with Q1.
- DE4, *Ernest's*: the configuration directory has no customary name or place. **Ernest**. A configuration directory has no customary name, so a repository cannot keep it out by name.
- SE1, *Ernest's*, the session's, from Q6's trial: `ern doc --man` titles a library's module `Ernest.Name` in "Ernest Manual", as though it were Ernest's own. **Ernest**.
- DE5, *Ernest's*: a development build passes `ern build` as its release, so the Makefile matches the version text. **Drop**. The template passes a development build on purpose.

## K's list

Cold reader K, commit d8b7ab4, ern 0.11.0+93a13b13.

### What I did

Every command in the README's *Building* and *Running* was run except a release with the installed `ern`, which the Makefile refuses. All work was in the clone and under the review's K-work directory; `/home/jocke/src/ernest-template` is untouched.

- **The template as it stands:** `make`, `test`, `examples`, `run`, `doc`, `release`.
- **An application, `greeter`,** begun by the README's last section, with an `examples/`, a `test/`, a package and an Erlang application under `erl/`.
- **A library, `word_list`,** begun the same way, released, and named in `greeter`'s `package.conf`.
- **Release, install and uninstall,** under scratch prefixes, from a checkout and from an unpacked archive.

Three things limit what the findings rest on:

- **The release path ran through a stand-in.** `K-work/release-ern/ern` is a wrapper that prints `ern 0.11.0` for `--version` and otherwise runs the installed `ern`. K7, K10 and the release half of K4 rest on it.
- **I read code, not working documents.** I read the `Makefile`, `bin/name`, `src/name.ern`, `package.conf`, `LICENSE`, `CHANGES.md`, `SECURITY.md`, `assets/README.md` and the two issue templates. I grepped `tools/docs.ern` for message lines only, and read nothing under `docs/`, nor `CLAUDE.md`, `TEMPLATE.md` or `TEMPLATE_LOG.md`.
- **Two claims are not run.** K24 (a later `ern`) and the macOS half of K19 are from reading alone.

### Defects

**K1. Step 2's `make test` cannot pass until steps 3 and 6 are done.**
- Place: `README.md:53`, "Write `src/<name>.ern` … with its first test, and `make test`."
- Shown by: after steps 1 and 2 with one test citing `// design §1`, `make test` ends with
  ```
  README.md: `bin/name` names nothing
  TEMPLATE.md: `bin/name` names nothing
  TEMPLATE.md: `src/name.ern` names nothing
  docs/design.md: §2 has no test naming it
  docs/design.md: §3 has no test naming it
  ```
- What is wrong: the first line is step 1's own sentence. The others go only once the design is rewritten (step 3) and the template's notes are removed (step 6).
- Fix: move `make test` to the end of step 6, or have step 2 say which lines remain until then.

**K2. "A clone with its `.git` removed" fails `make test`, and after `git init` the documents' check reads nothing and passes.**
- Place: `README.md:50`; `tools/docs.ern:148`.
- Shown by: `rm -rf .git; make test` gives `docs: git ls-files failed` and Error 1. After `git init` with nothing staged, I appended a 200-word paragraph to the README, removed `docs/design.md` and added `// Milestone 2 added this.` to `src/name.ern`; `make test` exited 0. After `git add -A` the same tree fails with four lines.
- What is wrong: the README never says the check reads tracked files alone, and the check does not say when it read none.
- Fix: the step says `git init` and `git add -A` before `make test`, and `docs.ern` refuses with a sentence when no file is tracked.

**K3. In the unpacked archive of a program with an Erlang application, `make`, `make run` and `make doc` fail with advice that cannot be followed.**
- Place: `Makefile:93-97`; the comment at `Makefile:178` says the archive carries the Makefile "so that make install and make run run in it".
- Shown by: `greeter` with `ERL_DEPS = loud`, released and unpacked. `make run` gives `erl/loud is empty: git submodule update --init` and Error 1. `bin/greeter` and `make install` do work there.
- What is wrong: the archive has no `erl/` and no git, only `ebin/` at its top, yet `lib` loops over `ERL_DEPS`.
- Fix: `lib` skips the loop where there is no `erl/`, as the `erlang` function already does.

**K4. `make -j` fails from a clean tree that names a package.**
- Place: `Makefile:86`, `all: lib build`.
- Shown by: `make clean; make -j4` in `greeter`, three runs of three: `ern build: package.conf: word_list 0.1.0 is not under lib; ern unpack puts it there`. Serial `make` passes.
- What is wrong: nothing orders `build` after `lib`. `release: test doc` is unordered in the same way.
- Fix: `.NOTPARALLEL:`, or `build: lib`.

**K5. An installed launcher reached through a symbolic link does not find the program.**
- Place: `bin/name:11`, `here=$(cd "$(dirname "$0")/.." && pwd)`.
- Shown by: `ln -s $PREFIX/bin/greeter ~/bin/greeter; greeter Ada` gives `ern run: …/package.conf: no such file`, status 1.
- What is wrong: the launcher takes the link's directory for its own, and the message names a file the user never heard of.
- Fix: resolve `$0` through its links before taking its directory, or refuse with "run it by its own path".

**K6. `make release` ships the compiled form and the page of a module git does not track.**
- Place: `Makefile:191` and `Makefile:200`, against the comment at `Makefile:74-76`, "so that no untracked file goes in".
- Shown by: an untracked `src/word_list/scratch.ern`, then `make release`. The archive holds `build/word_list/scratch.erc` and `docs/man/word_list/scratch.md`, and no source for either.
- Fix: release refuses where `src/` holds an untracked `.ern`, or copies only the `.erc` of each tracked source.

**K7. A library module named `index` loses its page, and the archive's `docs/man/README.md` links to it.**
- Place: `Makefile:200`, `! -name index.md`, which matches at every depth.
- Shown by: `src/word_list/index.ern`, then `make release`. `docs/man/README.md` lists `[WordList.Index](word_list/index.md)` and the archive holds no such file.
- Fix: exclude `./index.md` by path, not by name.

**K8. `bin/<name> --config-dir` with no directory answers in the shell's words.**
- Place: `bin/name:16-18`.
- Shown by: `bin/greeter --config-dir` gives `bin/greeter: 18: shift: can't shift that many`, status 2.
- Fix: `[ $# -ge 2 ] || { echo "$name: --config-dir takes a directory" >&2; exit 2; }`.

**K9. `make clean` leaves what `make lib` built under `erl/`.**
- Place: `README.md:32`, "`make clean` removes what the build and `make lib` wrote"; `Makefile:242-245`.
- Shown by: after `make clean`, `erl/loud/ebin/loud.beam` is still there.
- Fix: the sentence says each application's own build stays, or `clean` runs each application's `make clean`.

**K10. `make release` refuses a build of `ern` that is no release only after it has run the tests and written the pages, and the README never says it refuses one.**
- Place: `Makefile:185-187`; `README.md:23`.
- Shown by: `ERN=$HOME/opt/ernest-0.11.0/bin/ern make release` runs `test` and `doc`, then `a release is not made with a development build of ern`, Error 1.
- What is wrong: the installation I was given says `ern 0.11.0+93a13b13`, which report §11.7 calls no release, so no archive can be made with it. The message says "development build" of what is an archive build from a commit.
- Fix: check first, name the version text in the message, and add "with a release of `ern`" to the README's line.

**K11. The checker says one fault of a module under `src/` twice.**
- Place: `tools/docs.ern`, the history check.
- Shown by: `// Milestone 2 added this.` in `src/greeter.ern` gives both `src/greeter.ern:38: a comment names a milestone` and `src/greeter.ern:38: the line names a milestone`. The same comment in `examples/card.ern` gives one line.
- Fix: a module's comment is read once.

**K12. `make test` in an unpacked archive fails with `ern format: tools: no such file`.**
- Place: `Makefile:107`. The archive carries the README, which lists every target, and no `tools/`.
- Fix: the README says which targets an unpacked archive takes (`make`, `make run`, `make install`), or `test` refuses there in a sentence.

### Clarity

**K13. `<name>` stays in a finished program's README.**
- Place: `README.md:36`, `README.md:40`, `README.md:52`.
- What is wrong: step 1 replaces `NAME`, so `bin/<name>`, "the installed `<name>`" and `src/<name>.ern` remain. A library also keeps the whole *Running* section and the `make run` and `make install` lines, which answer "is a library: nothing to run".
- Fix: step 1 names both spellings and says what a library removes.

**K14. Nothing in the tree says which tag of the template it is.**
- Place: `README.md:54`, "`docs/log.md`'s first entry names the template's tag".
- What is wrong: *Use this template* and a clone without `.git` both drop the tags. `VERSION` is the program's. Only `git describe` in the template's own clone told me v0.11.0.
- Fix: a file of the template holds its tag, or the step says where to read it.

**K15. The README does not say what an example is given.**
- Place: `README.md:21`, "each program of examples/ built and run, what it writes under build/examples/".
- What is wrong: only `Makefile:118-120` says a program is run with one argument, `build/examples/NAME` and `EXAMPLE_SUFFIX`, which it must write.
- Fix: one sentence in the README.

**K16. "`test/` … holds a program run end to end" does not say what to write.**
- Place: `README.md:42`.
- What is wrong: I guessed modules of `Test.Case` that run `bin/greeter` by `Os.run`, with the checkout as the working directory. That worked. A program with `main` put there would be built and passed over in silence.
- Fix: say what a module under `test/` holds and where it runs.

**K17. The form of a design citation is nowhere in the README.**
- Place: `README.md:16` and `README.md:53`.
- What is wrong: I learned `// design §N: …` from the placeholder's comment in `src/name.ern`, and that every numbered section needs one from the failure in K1. I wrote `docs/design.md` blind as `## 1. Greeting`, which passed.
- Fix: step 2 or 3 gives the comment's form and the rule.

**K18. "Names the project's history" does not say what is refused.**
- Place: `README.md:17-18`.
- What is wrong: by trial, `Milestone 2`, a date such as `2026-11-01` and "`docs/plan.md`'s item 4" are refused in a comment. `M2`, `Step 3 of the plan`, `Since v0.2.0`, `issue #12` and "used to be called" pass. A string the program prints is "text a user reads" and is not read at all.
- Fix: name the kinds in the README.

**K19. What the build needs beyond `ern` is not listed.**
- Place: `README.md:11`.
- What is wrong: `make test` needs git (`tools/docs.ern:144`, `Makefile:70`). `make release` needs `cpio` and `sha256sum` (`Makefile:192`, `Makefile:204`). macOS has no `sha256sum`; I did not run there.
- Fix: list them, or use `tar` and `shasum -a 256`.

**K20. The launcher needs `ern` on `PATH`, or `ERN` in its environment, and *Running* does not say so.**
- Place: `README.md:36`; `bin/name:24`.
- Shown by: after `ERN=… make`, `bin/greeter Ada` gives `bin/greeter: 24: exec: ern: not found`, status 127.
- Fix: one sentence, and that the launcher reads `ERN`.

**K21. `make run` passes the program no argument.**
- Place: `README.md:22`; `Makefile:134`.
- Shown by: a program that needs one ends `make run` with its usage line and Error 2.
- Fix: `make run ARGS=…`, or say that arguments go through `bin/<name>`.

**K22. `src/name.ern` is never said to go.**
- Place: `README.md:53`.
- What is wrong: only the placeholder's own comment says to rename it. Left in place it keeps citing §1, §2 and §3, so the design check passes on a placeholder, and it ships.
- Fix: "rename `src/name.ern`".

**K23. A `priv/` in another application is refused only at install and release, and the remedy is not explained.**
- Place: `README.md:55`, "an Erlang application as a submodule under `erl/` of the application's name"; `Makefile:151-155`.
- Shown by: `erl/loud/priv` passes `make test`, then `make install` says `erl/loud has a priv/, which the host finds here only for the application greeter: make loud a package`.
- Fix: say the rule in step 4, and how an Erlang application becomes a package.

**K24. An unpacked release runs only under the build of `ern` that compiled it; not run.**
- Place: `README.md:11`, "or a later one"; `README.md:36`, "from an unpacked release alike"; `Makefile:211`, "Nothing is built here".
- What is wrong: report §11.2 refuses a form another build compiled, `compiled by another build of ern`. I had only one build, so this is from reading.
- Fix: say `make` comes first under another `ern`, which K3 must allow.

**K25. `docs/man/` holds CommonMark.**
- Place: `README.md:32`, "a library's archive carries the pages under `docs/man/`".
- What is wrong: `man` reads none of them, though `ern doc --man` writes real pages.
- Fix: name the directory for what it holds, or ship the `--man` pages.

**K26. `LICENSE` keeps the template author's copyright line.**
- Place: `README.md:55`, "0BSD as the template has it"; `LICENSE:1`, the template author's copyright line.
- Fix: "with its year and holder".

**K27. Small matters.**
- `README.md:57`: "the line under the title" is the epigraph on line 3; the line meant is line 5. Whether the epigraph stays is unsaid.
- `README.md:21`: `make examples` with no example is an error, `no program under examples/: nothing to build`, Error 1.
- `README.md:55`: `ACKNOWLEDGMENTS.md` "appears with the first name", and `Makefile:68` neither installs nor releases it.
- A two-module library's archive is 550 KB, nearly all of it `assets/*.png`, and every dependent's `lib/` and installation carries them.
- `Makefile:107-108` echo `ern format --check src tools  ` and `ern test  build` with stray spaces.

### Ernest's, not this repository's

**E1. `ern doc src` overwrites the page of a root module named `index` with its listing, in silence.**
- Shown by: `src/index.ern` and `src/other.ern`, then `ern build --build-root build src; ern doc --build-root build src`. Status 0, and `build/index.md` is the listing, which links `[Index](index.md)` to itself.
- Ask: refuse the module, or name the listing so that no module can take its name.

**E2. `ern doc` has no place for the pages apart from the `.erc`.**
- `--build-root` names both. The template sifts `*.md` out of `build/` by `find` with three exclusions (`Makefile:200`), which is where K7 comes from.
- Ask: `--doc-root dir`.

**E3. The library lacks the index of the first element a test passes.**
- `List.findIndex` is `unknown name`, and the diagnostic has no help line, though `List.find` and `List.indexed` stand beside it.
- I wrote `Optional.map(List.find(List.indexed(list), fn(#(_, other)) = other == word), fn(#(index, _)) = index)`. One site.

**E4. `ern format --check` answers with a bare path.**
- `src/greeter.ern` was the whole output. The Makefile's echo was the only context that told me it meant "not laid out".

**E5. `ern format` hangs a long call's arguments under its bracket.**
- In `test/end_to_end.ern` the body of `run = fn() =` begins at column 46 and the innermost tuple at column 47. I had written one item a line at four spaces, and it was rewritten.
- The style guide's answer is to name a part, which a test of one expression should not need.

**E6. The installation's version text is `0.11.0+93a13b13`.**
- Report §11.7 calls that no release, and it is why K10's refusal fires. A user who installed from this archive cannot release an application.

**E7. The guide points outside the installation.**
- Guide §7.1 sends the reader to `https://github.com/joagre/ernest/blob/93a13b13/docs/module_doc_template.md` for what a module's documentation holds. I wrote doc blocks from report E.0 rule 6 alone.

**E8. Forms repeated in the Ernest I wrote** (three modules of `greeter`, three of `word_list`):
- `let x = Test.Case(name = "…", run = fn() = Test.equal(…))`: 7 sites of mine. A grep counts 21 in `tools/docs.ern` and 1 in `src/name.ern`.
- `Io.printlnError(text); Os.exit(status)` in a block: 3 sites.
- `Fs.write(Path(path), …, 5000)` matched on `Right(Unit)` and `Left(error)`: 2 sites, one of them with `String.toUtf8` first.
- `Either.map(Os.run(Os.command(…), ms), fn(finished) = #(finished.status, String.fromUtf8Lossy(finished.stdout)))`, to compare a program's status and output as text: 1 site.

**E9. Messages that needed no guessing.** `ern unpack`'s three refusals (no archive, no `sha256`, a wrong digest), `ern build`'s `written for ern from 0.12.0, and this is ern 0.11.0+93a13b13`, and `ern: no job frob` each said what to do.


## C's list

In the commands below, E is `$HOME/opt/ernest-0.11.0/bin/ern`. Every run was in my clone at d8b7ab4, built by `ERN=E make`, and P is a scratch PREFIX. I ran `make release` with the development-build check at Makefile:186 edited out, because this ern prints `0.11.0+93a13b13`. I left both the clone and /home/jocke/src/ernest-template clean. `make test` passes at d8b7ab4.

**Defects**

C1. Makefile:216-219 and 233-235, `@test -d $(TREE) || test ! -e $(PREFIX)/bin/$(NAME) || …` and then `rm -rf $(TREE) $(DOC_DIR)`.
- What is wrong: any directory at PREFIX/lib/NAME is taken for this program's installation. `install` removes it whole, removes share/doc/NAME without any check, and overwrites the launcher; `uninstall` does the same. The refusal of "a launcher of another program's" holds only where no such directory stands. Ernest installs itself as PREFIX/lib/ernest.
- Shown: `mkdir -p P/lib/name P/share/doc/name; echo keep > P/lib/name/precious; echo keep > P/share/doc/name/other.txt; make install PREFIX=P` exits 0, and both files are gone.
- Fix: before anything is removed, refuse a TREE that holds no package.conf and build/NAME.erc, or a marker that install writes.

C2. Makefile:144-147, `cp -RL "$${dir%/}" $(1)/lib/`.
- What is wrong: report §11.9 allows a named package that is a link. Such a package is copied whole into the published archive and into the installation, with its .git/, an .env and its own lib/ archives.
- Shown: lib/leaf linked to a directory holding .git/config, .env and lib/dep-1.0.0.tar.gz, then `make release`. `tar tzf build/name-0.1.0.tar.gz` lists name-0.1.0/lib/leaf/.git/config, …/.env and …/lib/dep-1.0.0.tar.gz.
- Fix: copy only what §11.9 says a package is (package.conf, VERSION, src/, build/, ebin/, priv/), or refuse a linked package at release.

C3. Makefile:185-205, `release`.
- What is wrong: SOURCES and DOCS are read from the working tree, and nothing checks that it is committed. An archive published beside a signed tag can hold what the tag does not.
- Shown: with package.conf edited and not committed, `make release` exits 0 and the archive holds the edited package.conf.
- Fix: in a checkout, refuse where `git status --porcelain --untracked-files=no` prints anything.

C4. Makefile:93-96, the `lib` loop in an unpacked archive.
- What is wrong: the archive carries the Makefile and its ERL_DEPS but no erl/. So `make` and `make run`, which TEMPLATE.md §4 says run there, stop at the loop with "erl/foo is empty: git submodule update --init".
- Shown: the archive's layout with no erl/, `make run ERL_DEPS=foo` prints that line and exits 2.
- Fix: run the loop only `if test -d erl`, as the `erlang` macro does.

C5. Makefile:86, `all: lib build`.
- What is wrong: `build` does not depend on `lib`, so `make -j` can compile before anything is unpacked.
- Shown: one package in package.conf, `make clean; make -j2` gives "ern build: package.conf: leaf 0.1.0 is not under lib; ern unpack puts it there" and exits 2.
- Fix: `build: lib`.

C6. bin/name:15-19 and 23, `config=$2; shift 2` … `[ -n "$config" ] && set -- --config-dir …`.
- What is wrong:
  - `bin/name --config-dir "" x` runs the program, silently not as a node. ern itself refuses an empty value (§11).
  - `bin/name --config-dir` with no value: under dash it prints "bin/name: 18: shift: can't shift that many" and exits 2. Under a bash /bin/sh it passes `--config-dir` to the program as an argument and exits 0.
- Shown with a fake ERN that prints its arguments.
- Fix: where `$# -ge 2`, forward `--config-dir "$2"` whatever its value. Otherwise refuse with "--config-dir takes a value: --config-dir dir".

C7. tools/docs.ern:763-817, `historyAt`, `stepAt` and `noteAt`, which `timeline` (705-710) applies to every line under src/.
- What is wrong: history is read by plain English words, so a program whose domain has milestones, plans, page sizes, function keys or dates cannot write its own code:
  - `type Milestone = …` is "the line names a milestone";
  - "(A4)" is "a review's finding";
  - "the plan, the stops and the legs" is "a plan item";
  - "since 2026-03-29" is "a date";
  - a feed reader's release note, "the reader now…", is "a reader".
  A copy cannot change the checker, since it is the template's.
- Shown: append those lines to src/name.ern and run `E run tools/build/docs.erc`. It reports six findings and exits 1.
- Fix (a decision for the user): refuse only the project's own forms, such as `MVP n`, the plan's milestone headings read from docs/plan.md, a finding's name after "finding", and `the log's *…*`. Do not refuse the bare words.

C8. tools/docs.ern:254-255, `file != "docs/plan.md" && file != "docs/findings.md"`.
- What is wrong: a proposal names paths not yet written, as the plan does, and the log names paths that were there when it was written. Both are still checked.
- Shown: a tracked docs/proposals/cache/proposal.md naming `src/cache.ern`, and a log entry naming `src/old_parser.ern`. Each "names nothing", and the run exits 1.
- Fix: leave out docs/log.md and docs/proposals/ too, as `isMeasured` does.

C9. tools/docs.ern:495-501, `unquoted`.
- What is wrong: the comment lines are taken out of the module but not out of the part. A part quoted byte for byte with a comment line is refused, a function with its doc block among them.
- Shown: a README ernest block copying src/name.ern's lines 13-15 gives "README.md:10: a part of an Ernest block stands in no tracked module".
- Fix: hold the part against the module as written as well as without its comments.

C10. Makefile:211-212, "Nothing is built here, so that an archive installs as it was compiled".
- What is wrong: §11.2 refuses a compiled form that another build of ern wrote, "another version or the same version's code changed", and the installation holds no source. So an installed archive runs only under the ern build that made the release. TEMPLATE.md §4's "under any release of its floor" contradicts §11.2. In a checkout, `install` copies a build/ older than src/, since it checks only `test -f`.
- Not run: I had only one ern.
- Fix: have `install` run `ern build src` first, which recompiles only what is stale; or say this limit in the README and TEMPLATE.md.

C11. bin/name:11, `here=$(cd "$(dirname "$0")/.." && pwd)`.
- What is wrong:
  - Reached through a link of its own name (L/name → P/bin/name), the run fails with "ern run: package.conf: no such file" and exits 1.
  - With CDPATH exported naming a directory that holds bin/, the root becomes that directory, written twice and joined by a line feed.
- Shown: both runs, the second with `CDPATH=$W/cdp:.` and a $W/cdp/bin.
- Fix: `CDPATH= cd -P -- "$(dirname -- "$(realpath -- "$0")")/.." >/dev/null && pwd`.

C12. Makefile:195-196, `test -x bin/$(NAME) && mkdir -p … && cp … || true`.
- What is wrong: the `|| true` that stands for a library also hides a failed copy, so the archive ships without its launcher.
- Shown: `chmod 100 bin/name; make release` prints "cp: cannot open 'bin/name' for reading: Permission denied", exits 0, and the archive has no bin/name.
- Fix: `if test -x bin/$(NAME); then mkdir -p … && cp …; fi`.

C13. tools/docs.ern:211-246 and 302-332, the checker's own Markdown reading.
- What is wrong:
  - One lone backtick flips the parity of `String.split(…, "`")`, and no path after it is checked.
  - `isFence` toggles on any ``` or ~~~ line, so a four-backtick fence that quotes a three-backtick block flips the state.
  - `isUnmeasured` reads the untrimmed line, so a table row indented under a list item is measured as prose.
- Shown, each appended to CHANGES.md:
  - "A lone ` mark.\n\nSee `docs/nosuch.md`." exits 0, the missing path not found;
  - a ```` fence holding ``` and `docs/nosuch.md`, then `docs/nosuch2.md` after it: the first is reported, the second is not;
  - "- an item\n\n  | cell | …" gives "CHANGES.md:7: 153 words".
- Fix: read the documents through Markdown.parse (Appendix G.2), which lacks positions (C47). Short of that: find code spans per paragraph, match a fence by its character and length, and test the trimmed line.

C14. tools/docs.ern:199-203, `Fs.stat(Path(path), 5000)`.
- What is wrong: a path is held to the working tree, not to what git tracks. A path to an untracked file passes for its writer and fails on the fresh clone that docs/release.md's step 1 makes.
- Shown: CHANGES.md naming `docs/notes.txt`; after `touch docs/notes.txt` the run exits 0, and after removing it the run reports "names nothing".
- Fix: under a tracked top, hold the path to `git ls-files`.

C15. tools/docs.ern:144, `Os.command("git", ["ls-files", pattern])`.
- What is wrong: git quotes a name past ASCII, and the checker cannot read the quoted name.
- Shown: a tracked docs/café.md gives `docs: cannot read "docs/caf\303\251.md": Io.NotFound` and exits 1.
- Fix: `git -c core.quotePath=false ls-files -z`, split at NUL.

C16. tools/docs.ern:185, `Io.printlnError("docs: not UTF-8")`.
- What is wrong: the message names no file.
- Shown: a tracked docs/latin1.md holding "caf\xe9" gives only "docs: not UTF-8".
- Fix: pass the file's name to `text`.

C17. Makefile:240-245, `clean`.
- What is wrong: it leaves what `$(MAKE) -C erl/$$app` wrote, though lines 29-30 say it removes what `make lib` wrote. It also removes every directory under lib/, which §11.9 allows a user to place by hand, though the comment calls these "the packages ern unpack wrote".
- Fix: run each application's `make clean`, and remove lib/<name> only beside lib/<name>-*.tar.gz.

C18. tools/docs.ern:632-636, `String.startsWith(line, "let ")`.
- What is wrong: an `export let` Test.Case, which Appendix A allows and §11.2 runs "exported or not", is no test to the checker. Its citations count for nothing.
- This is the one place the code does not keep docs/design.md's only rule, its introduction's.
- Fix: strip a leading "export " first.

C19. Makefile:185-187.
- What is wrong: `release` refuses a development ern only after `test` and `doc` have run.
- Fix: make the check a prerequisite that runs before `test`.

**Tests that pass with what they test broken**

C20. tools/docs.ern:936-942, `findsPaths`.
- What is wrong: the tops are ["src/", "docs/"], and `lib/*/build`, `bin/<name>` and `bin/a --config-dir …` begin with neither, so the wildcard, metavariable and space rules are never reached.
- Shown: delete lines 222-224; the whole suite passes.
- Fix: tops ["src/", "docs/", "lib/", "bin/"].

C21. tools/docs.ern:949-961, `findsCitations`.
- What is wrong: the rules of `listed` that a list needs its comma and that a citation stands on the same line or the next are never exercised.
- Shown: change 673 to `(if true then` or drop 669's guard; the suite passes either way.
- Fix: add "// design §2 §3" and a design word followed by § two lines later.

C22. tools/docs.ern:975-985, `findsTested`.
- What is wrong: no case puts a blank line between a comment and its test.
- Shown: change line 620 to `#(above, tested)`; the suite passes.
- Fix: add "// design §6\n\nlet t = Test.Case(…)", expecting no 6.

C23. tools/docs.ern:992-1045, `findsHistory` and `findsNotes`.
- What is wrong: each refused line carries several forms of one kind, and `List.unique` folds them into one finding. The test's own comment admits it.
- Shown: removing any one of these alone leaves the suite passing: `raw == "plan,"`; the `(plan` form; `docs/plan.md`; `findings.md`; the parenthesized finding form (777-779); `noteAt`'s lowercase "review".
- Fix: one refused form per line.

C24. tools/docs.ern:911-923, `readsItems`.
- What is wrong: "plain after" is two words, so the test's result is the same with the item's indentation rule removed (line 306). Only `leavesUnmeasured` catches it.
- Fix: make the line after the item long.

C25. src/name.ern:13-15, `Test.equal(1 + 1, 2)`.
- What is wrong: the test passes whatever the module does. In a copy that forgets it, it keeps §1 to §3 "tested" for the checker.
- Fix: `Test.capture(main)` against "name: nothing yet\n", which fails once `main` is written.

**Comments that no longer hold**

C26. tools/docs.ern:10 and 45, "(CLAUDE.md, *Writing*)". CLAUDE.md states neither the 150-word measure nor the history rule; TEMPLATE.md:81 says "the file states neither". Fix: drop both citations.

C27. tools/docs.ern:17 "holds no two spaces before its `#`", and `isBare`'s comment at 466-467. README.md:14's own "make            # builds" has twelve. The code refuses two spaces within the command and lets the run of spaces before " #" through. Fix: say that.

C28. Makefile comments:
- 66-67 "EXAMPLES_MADE's, which make release wrote": release never writes examples/build into the archive.
- 228-231 "and nothing else" stands beside "whoever made it", and against C1.
- 142-143 (C2) and 29-30 / 240-241 (C17) do not say what the code does.

C29. tools/docs.ern header, code it does not state:
- "Every backticked path" (4): `pathsIn` also passes over wildcards, metavariables, spaces and a trailing "/".
- The citation rule (36-37) does not say that a citation may follow "(design" or stand on the next line.
- "names no step of the plan or item of it" (47-48) does not cover "plan," and "(plan" (770-771), which the code refuses.

**Clarity: shorter and clearer**

C30. tools/docs.ern, 22 sites of `… == false` (159, 221-225, 232, 260, 290, 319, 418, 422, 430, 442, 464, 513, 530, 532, 584, 627, 756, 847). Ernest negates with prefix `!` (report §2.6), and `!String.startsWith(…)` compiles. Fix: `!`.

C31. tools/docs.ern:114-136 and the checks. `main` reads the modules once, but each document is read again by each check: `contents` is called at 200, 263, 396, 487, 558 and 700, and README.md is read up to four times. The reading, with its `Os.exit`, is spread across ten functions named as nouns (tracked, directories, contents, text, missingIn, paragraphsIn, commands, quoted, uncited, timeline), against style.md's "A function that does something is a verb". Fix: read every document once in `main` and keep the checks free of reading.

C32. tools/docs.ern:228-246, 288-298, 414-423 and 527-533. Four fence trackers each toggle `fence == false`, and three state records each end in `List.reverse`. Fix: one pass that tags each line with its fence and language (or Markdown.parse, C13).

C33. tools/docs.ern:111-112, `notice` writes "150" again beside `measure`, and the bound 5000 is a bare literal at 144, 156, 171 and 200. Fix: `Int.toString(measure)`, and one named `ms`.

C34. tools/docs.ern:254 `isChecked` and 361 `numbered` sit under the *The paragraphs* banner, though their only users are the paths check and `sectionsOf`. Fix: move each to its user, as style.md asks.

C35. tools/docs.ern:
- 361-365, 685-691 and 798-799 slice by `String.size` where `String.stripSuffix(word, ".") |> Optional.andThen(String.toInt)` and `String.stripPrefix` would do;
- 457 `program :: _ when program == "make"` is `"make" :: _`;
- 229-240 use one-clause `match acc` and `match kept` where `let #(…) =` or a parameter pattern is used elsewhere in the module.

C36. tools/docs.ern:98, 519, 547 and 304. "Nothing begun" is a sentinel, `Part(line = 0, lines = [])` and `words == 0`, where `Optional(Part)` and `Optional(Paragraph)` would say it in the type.

C37. tools/docs.ern:202. "names nothing" is the one finding with no line number, because `pathsIn` joins the text. Fix: read per line.

C38. Makefile:
- 73 `$(foreach dir,$(EXAMPLES_MADE),…)` runs over a single value;
- 190-192 (find -prune | cpio) and 222 (find ! -path | tar | tar) are two ways to copy the .erc, with different exclusions;
- 60-67, the DOCS comment, is one eight-line sentence.

C39. tools/docs.ern:875-1138. The checker's tests are documented with `///`, the form its own rule (602-603) says carries no citation, so a copy that learns from the checker learns the wrong form. Fix: use `//`.

**Names**

C40. tools/docs.ern:483 `quoted` answers the parts that are *not* quoted, and 394 `commands` answers the lines that break the rule. Fix: name each for what it answers.

C41. `read` names three things: the paragraph step (288), `CommandReading.read` (90), and `timeline`'s local (699), which shadows the step. Fix: give each its own name.

C42. 755 `sectionsIn` answers a note's lines, and 573 `sectionsOf` answers the design's section numbers. Fix: rename `sectionsIn` to `notesIn`.

C43. 863 `isNumber` asks only whether a word begins with a digit, so "4abc" counts. Fix: rename it `beginsWithDigit`.

C44. 259 `isMeasured` also chooses the files whose commands are read (395), and 254 `isChecked` does not say what is checked.

C45. `line` is a line's text at 288, 302 and 414, and its number in Reading, Paragraph, Word, Citation, Part and `placeOf`. A line's number is also called `start` and `number`. `words : Int` is a count, which the glossary calls a count.

C46. `Reading.skip`, `timeline`'s local `printed`, `sectionsIn`'s `isProse`, `naming`'s `what`, and `timeline` itself do not say what they are.

**Ernest's**

C47. Appendix G.2, `Markdown.parse : (String) -> List(Block)`.
- What is wrong: the blocks carry no position, so a tool that must say file:line cannot use Ernest's CommonMark reader. It writes its own instead (C13, C32), which CLAUDE.md calls a library's work. Principle 2.
- Ask: each Block's line, counted from 1.

C48. `ern test` over a directory runs a .erc under a directory that breaks §11.1's path shape, though §11.2 says it finds modules "as ern build finds the sources".
- Shown: `ern build src` with src/v-1.0/a.ern refuses with "path component `v-1.0` must be words joined by `_`…" and exits 1. With out/v-1.0/a.erc, `ern test out` prints "A / t: passed" and exits 0.
- Here: a failed release leaves build/name-0.1.0/build/name.erc, and `make test` then runs every test twice.

C49. The installation prints `ern 0.11.0+93a13b13`, which §11.7 calls "no release". The template's `make release` rightly refuses it, so no copy can make a release with the only installation the session may use. Either the 0.11.0 archive was cut away from its tag, or this installation is not that release.

C50. Forms repeated at site after site:
- shape rule 8 asks a time of every local `Fs.read`, `Fs.stat` and `Fs.list`, and the checker writes 5000 at three such sites, with no other party to bound;
- `List.indexed` counts from 0 while every finding names a line from 1, so `index + 1` is written at five sites (284, 410, 523, 649, 721).

These are mild, and I make no ask.

## D's list

D, the documents reader, at d8b7ab4: 12 defects, 14 matters of clarity, 5 findings of Ernest's.

Read: the twelve documents named, with `Makefile`, `bin/name`, `package.conf`, `.gitignore`, `.github/`, `src/name.ern` and `tools/docs.ern` where a document claims something of them, against `~/opt/ernest-0.11.0/share/doc/ernest/`. Nothing was edited in the repository.

Ran, all in the clone: `make test` (passes), `make run`, `make doc`, `make install PREFIX=<scratch>`, `make clean`. `make release` refuses the installation's `ern`, so I made the archive through a stand-in `ern` that answers `--version` with `ern 0.11.0`; then tried it unpacked, installed, and as a consumer's dependency.

Not checked: any claim that needs a second build of `ern` (D1's refusal, and README.md:11's `ern: no job unpack`), and `priv/` lookup, which needs an Erlang application.

### Defects

**D1. TEMPLATE.md:71 (§4), with TEMPLATE.md:69, Makefile:207-212, README.md:36.**
- Quote: "the compiled modules travel so that an operator runs the application as it is, under any release of its floor"; "It builds nothing, so that an archive installs as it was compiled".
- Wrong: report §11.2 refuses a compiled form another build of `ern` wrote, "another version or the same version's code changed", with `ern run: main.erc: compiled by another build of ern`. Ernest's `CHANGES.md` (0.10.0) says the same. A floor (§8.7) is about nodes connecting, not about loading a `.erc`.
- Consequence: `bin/<name>` in an unpacked archive, and `make install` from one, run only under the very build of `ern` that made the release. An installation stops at the operator's next `ern`, and holds no source of the program to build again.
- Shown by: the report's sentence only; the installation holds one `ern`.
- Fix: say the compiled modules run under the `ern` that built them alone, and have README's *Running* tell an operator to run `make` in the unpacked archive first (or make `install` depend on `all`).

**D2. TEMPLATE.md:24 (§2), TEMPLATE.md:47 (§3), .gitignore:8-9.**
- Quote: "started with `--config-dir dir` (§8.3, §11.3), whose `.ernest/` holds a private key"; "A node's configuration directory holds a private key / `.ernest/`".
- Wrong: by report §11.3 the configuration directory is whatever `--config-dir` names, and holds `private-key.pem`, `certificate.pem` and `ernest.conf`. `.ernest` is only `$HOME/.ernest`, the shell's history and startup (§11.2).
- Consequence: a directory made by `ern config --config-dir node` in a checkout is not ignored, and its key can be committed.
- Shown by: `grep -rn '\.ernest' ~/opt/ernest-0.11.0/share/doc/ernest | grep -v 'HOME/.ernest\|/home/ada'` prints nothing.
- Fix: drop "whose `.ernest/`", and either ignore `private-key.pem` or say a configuration directory stands outside the checkout.

**D3. docs/full_review.md:20 against docs/agents.md:17.**
- Quote: "A reader hands its list back as text and writes it to a file under the review's session's scratchpad, as `agents.md` says of an agent."
- Wrong: `agents.md` says the opposite: "an agent cannot write a file of its report. The session keeps what it needs of it in a file under its scratchpad".
- Fix: "A reader hands its list back as its answer, and the session keeps it, as `agents.md` says."

**D4. docs/full_review.md:16.**
- Quote: "with the `ern` the Makefile names".
- Wrong: stale. The Makefile names no release; `package.conf` does.
- Shown by: `grep -n ERN Makefile` gives only `ERN ?= ern`.
- Fix: "with an `ern` of the release `package.conf` names".

**D5. docs/full_review.md:13 and docs/release.md:5.**
- Quote: "`git clone`, with `--recursive` where there is an `erl/`, then `make test`"; "A fresh clone builds and passes".
- Wrong: `lib/` is ignored and no job reads the network, so a fresh clone of a program that names a package stops at `make lib`.
- Shown by: a clone whose `package.conf` names `leaf 1.2.0`, then `make test`: `ern unpack: package.conf: leaf 1.2.0 is not under lib; download https://example.org/leaf/leaf-1.2.0.tar.gz to lib/leaf-1.2.0.tar.gz`, `make: *** [Makefile:92: lib] Error 1`.
- Fix: add "each archive `ern unpack` names put under `lib/`" between the clone and `make test`.

**D6. TEMPLATE.md:63 (§4), README.md:53 (step 2); no document owns the rule.**
- Quote: "One shape for an application and a library, so that any archive can be a dependency".
- Wrong: report §11.9 holds every module under a named package's `src` to the package's namespace. No document tells a copy that its modules stand at `src/<name>.ern` or under `src/<name>/`, and `make test` does not hold it.
- Shown by: the release archive with `src/util.ern` added, named by a consumer; `ern unpack` takes it, then `ern build src` says `ern build: lib/name/src/util.ern: the package name provides Name and what stands under it`. The unchanged archive builds and runs as a dependency.
- Fix: state the rule in README's step 2 and in TEMPLATE.md §3, or narrow "any archive" to one whose modules stand under its name.

**D7. CLAUDE.md:26, CLAUDE.md:54, TEMPLATE.md:11, docs/README.md:13.**
- Quote: "a line each until Ernest answers"; "A line the next release answers goes … and one not agreed with stays, the verdict and the reason beneath it"; "a line is carried there … and then goes, and the file goes when it is empty".
- Wrong: three lifetimes for a line of `language_feedback.md`: until carried, until answered, until a release answers it (and forever where refused). That the file goes when empty is said only in TEMPLATE.md, which a copy removes.
- Fix: keep CLAUDE.md:54 as the owner; make CLAUDE.md:26 and TEMPLATE.md:11 point at it.

**D8. TEMPLATE.md:7 (§1).**
- Quote: "no Erlang of its own, no readers of a language, and no section numbers for tests to cite".
- Wrong: §4 speaks throughout of "the program's own Erlang" under `erl/`. TEMPLATE.md:77, `docs/design.md`:3 and `src/name.ern`:13 have tests cite `design §n`, which `make test` holds.
- Fix: cut both phrases.

**D9. TEMPLATE.md:22 (§2), with Makefile:50-52.**
- Quote: "and a NIF's library from `priv/` beside `ebin/` (§8.4, §11.2)".
- Wrong: neither section says it. The report names `priv` once, at §11.9, of a named package only, and never a NIF.
- Shown by: `grep -n '\bpriv\b' report/*.md` gives toolchain.md:657 alone.
- Fix: cite §11.9 for a named package and call the rest the host's rule; it is also a line of `language_feedback.md` (E2).

**D10. README.md:32 and Makefile:29, against Makefile:242-245.**
- Quote: "`make clean` removes what the build and `make lib` wrote".
- Wrong: `make lib` also runs each Erlang application's `make` under `erl/` (Makefile:93-97), and `clean` removes nothing there.
- Fix: say "and leaves what each application under `erl/` built", or have `clean` run each one's `make clean`.

**D11. CLAUDE.md:52, README.md:11, TEMPLATE.md:25.**
- Quote: "written for one release of `ern` and those after it"; "the release `package.conf` names or a later one"; "a release of `ern` may refuse a program the previous release accepted, so an application is written for one release of `ern`".
- Wrong: two documents promise later releases, and the third gives the reason they cannot be promised.
- Fix: one sentence, owned by CLAUDE.md: `package.conf` names the least release, and a later one may refuse the program until it rises to it.

**D12. tools/docs.ern:10-11 and :44-45, against TEMPLATE.md:81 and CLAUDE.md:81-85.**
- Quote: "The project's history stays out of the code and of what a user reads (CLAUDE.md, *Writing*)".
- Wrong: *Writing* states neither that rule nor the 150 words, and TEMPLATE.md:81 says so: "the file states neither".
- Fix: drop the two citations.

### Clarity, restated facts and lists in two places

**D13. TEMPLATE.md:89 (§6) against docs/release.md:5-11.** The release's steps are listed twice. TEMPLATE.md leaves out step 4, the round, and puts the note after the tag where release.md commits it before. Fix: have §6 point at release.md.

**D14. docs/release.md:9, CHANGES.md:3, TEMPLATE.md:93.** The note's contents are stated three times. Only release.md has "the design's diff between the last release's tag and this one's", which does not say whether the diff or its command goes in the note. Fix: release.md owns it and says "the command that shows the design's diff"; the other two point.

**D15. README.md:11, .github/ISSUE_TEMPLATE/defect.yml:17, against package.conf:2.** "`ern 0.11.0`", "before 0.11.0" and "ern 0.11.0, OTP 29" restate `package.conf`'s `ernest`, and nothing holds them to it when it rises. Fix: README says "the release `package.conf` names" without the number.

**D16. CLAUDE.md:36, TEMPLATE.md:107, docs/full_review.md:45 (and `docs/log.md`:7).**
- The four files that are the template's are listed four times.
- No document says how a copy takes a change to the rest that TEMPLATE.md:51 and Makefile:1-3 call "the same in every application": the Makefile below its variables, `bin/name`, `docs/release.md`, `.gitignore`, the issue forms.
- Fix: CLAUDE.md:36 owns the list and names every such file; the others point.

**D17. CLAUDE.md:20-28, docs/README.md:5-16, TEMPLATE.md:41-45.**
- The catalogue of documents lives in three places.
- docs/README.md:3 says "What each document of this repository is", and README.md:40 and CLAUDE.md:96 send a reader there, yet it omits `SECURITY.md`, `assets/README.md`, `TEMPLATE.md` and `TEMPLATE_LOG.md`.
- CLAUDE.md:27 says "a review's findings"; full_review.md:9 says "a release's findings or a review's".
- Fix: docs/README.md lists every document; *Where a fact lives* keeps only owners.

**D18. Makefile:5-30, README.md:14-27, TEMPLATE.md:51.** The targets and what each does are listed three times, and differ on what `make test` checks. TEMPLATE.md counts "eleven targets"; `.PHONY` has twelve, with `build`. Fix: README's block owns what a user reads; TEMPLATE.md names no count.

**D19. TEMPLATE.md:59 (§4).** "**The floor.** `package.conf`'s `ernest` is the least release" uses a word the report defines otherwise (Appendix F: one major and minor release of `ern` on one major release of OTP), and TEMPLATE.md:23 uses it in the report's sense. Fix: head the paragraph "The least release".

**D20. `deploy/`: Makefile:62, TEMPLATE.md:67, docs/full_review.md:26 and :29.** Named four times and defined nowhere; TEMPLATE.md:43-45, "What appears when needed", omits it. Fix: one sentence there.

**D21. TEMPLATE.md §4 against README.md:57 (step 6) and docs/design.md.** The launcher's options, the archive's shape and the installation's layout are stated only in TEMPLATE.md §4, which a copy removes. In a copy only the Makefile's comments state them, though CLAUDE.md:13 makes the design the normative document. Fix: the starter design gains a section for them, or the README keeps what a user meets.

**D22. README.md:53 (step 2), src/name.ern:5-7, README.md:3.**
- The placeholder says "rename the file … as README.md's last section says"; the section says only "Write `src/<name>.ern`". A copy that leaves `src/name.ern` stays green, since its one test cites every section.
- No step and no document says what line 3, "*The Importance of Being Ernest…*", is or whether a copy keeps it.
- Fix: step 1 renames `src/name.ern` beside `bin/name`; TEMPLATE.md §3 gets a sentence for line 3.

**D23. docs/full_review.md:26, README.md:32, TEMPLATE.md:67.** "the manual pages `make doc` writes under `build/`", and `docs/man/`. `make doc` runs `ern doc src`, which writes CommonMark documents (`build/name.md`, `build/index.md`); report §11.4 keeps "manual page" for what `--man` writes. Fix: "the documents `make doc` writes".

**D24. TEMPLATE.md:79 (§5) against docs/release.md:9 and defect.yml:47.** "the design is not cited by number from outside", yet a release's note has "one line a change naming the design's section" and the issue form asks for "the design's section that states the rule". Both are outside, and `CHANGES.md` travels in the archive. Fix: say the citations are by title, or drop the reason.

**D25. Smaller.**
- CLAUDE.md:93 sends "Building, testing, running" to README's *Building*; running is *Running*.
- docs/agents.md:33 says "The stronger model" without saying stronger than which; agents.md:35 leaves the names to the session's memory, so a copy on another machine has none.
- TEMPLATE.md:67 says "`assets/`, whose pictures the documents show"; no tracked document shows either picture.
- docs/design.md:3 promises "its types", which no section holds.
- docs/full_review.md:3 says "all the code", yet no reader's list holds `package.conf`, `.gitignore` or `.github/`.
- docs/plan.md:5 restates CLAUDE.md:62's rule of the named decision.

**D26. CLAUDE.md:52 against TEMPLATE.md:59.** "installed from a release archive of Ernest's" beside "the applications are written against Ernest's unreleased builds". The `ern` this review was given is such a build (E1). Fix: say which holds while a release of `ern` is being driven.

### Ernest's

**E1. The installation is no release.** `ern --version` prints `ern 0.11.0+93a13b13`, which §11.7 calls no release. Its `CHANGES.md` has 0.10.0 as its newest section, though the README is headed "Ernest 0.11.0". Nothing in the installation says when `ern unpack` or §11.9 arrived, so README.md:11 cannot be checked from it. `make release` refuses it: "a release is not made with a development build of ern".

**E2. The report is silent on `priv` outside a named package.** §11.9 says the host finds a named package's `priv` beside its `ebin`. Nothing says so of an application under `--libs-dir`, or of an `ebin` that `--load-path` names, and "NIF" appears nowhere in report or guide. The launcher and the archive rest on both. Principle 3. Ask: a sentence in §11.2.

**E3. No way to carry a runnable program.** §11.2 refuses every `.erc` another build wrote, a patch release's among them, and `ern run` builds nothing. An archive or an installation runs under another `ern` only by carrying its source and building again (D1). The ask is the user's to decide: a rule for patch releases, or a sentence in the deployment guide saying an installed program is built by the `ern` that runs it.

**E4. The configuration directory has no customary name or place.** The report and the deployment guide give none, so a repository cannot ignore one by name; the template guessed `.ernest/` (D2). Ask: a sentence in the deployment guide on keeping it out of a checkout.

**E5. `ern --version` cannot be told from a release's by the three numbers.** `ern build` passes `0.11.0+93a13b13` as 0.11.0 (§11.9), so the Makefile matches `*-dev|*+*` on the text itself (Makefile:186-187). One site.

No message of `ern`'s was unclear. Each refusal met named its file and what to do.

One note for the session: the `CLAUDE.md` the harness handed me differs from the commit's at *The work*'s second rule. Mine read "one floor of `ern`, which the Makefile names"; the commit's reads "one release of `ern` and those after it, the release `package.conf` names". The working file equals the commit's, so the copy handed over was stale.

Scratch, all under the review directory: the clone is `D`; `D-work/consumer` and `D-work/two/consumer` are the two dependency trials; `D-work/floor` is D5's clone; `D-work/wrap/ern` is the stand-in.
