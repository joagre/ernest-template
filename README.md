# NAME

*The Importance of Being Ernest, a Trivial Comedy for Serious People*

> This is `ernest-template`, the repository an Ernest application is begun from. *Beginning from the template*, the last section, says how, and its last step removes this line.

What the program is, in a sentence a stranger can read, and what it does. Then one showing, before *Building*: a picture, a session, or a few lines quoted from the program's own source. Then where to begin. Nothing here argues what the program's documents argue. This repository was begun from [`ernest-template`](https://github.com/joagre/ernest-template), whose last section says how.

## Building

It needs [Ernest](https://ernest-lang.org) on your `PATH`, of the release `package.conf` names or a later one, and, in a checkout, git; `make release` needs `sha256sum` too. Before Ernest's 1.0 a later release may refuse the program, and the program is then brought to that release. Where an earlier release is found, `ern build` names both; an `ern` before 0.11.0 stops `make` sooner, at `ern unpack`, with `ern: no job unpack`. `ERN=path/to/ern make` names another `ern`: its directory stands first on `PATH` for everything the build starts, so whatever names `ern` by its name, a test or an example's shell, runs that one too. A file not called `ern` is not reached this way.

```
make            # builds: lib/ filled, each package and then the program compiled
make test       # in a checkout: the layout, every module's tests, test/ and the examples where they exist,
                # a dependent's build of the program, then the documents and the design's citations,
                # refusing any paragraph past 150 words, any comment or
                # text a user reads that names the project's history,
                # any command whose description stands without its #,
                # and any Ernest block of the README that no module holds
make examples   # each program of examples/ built and run, what it writes under build/examples/
make run        # runs the program through its launcher with the arguments RUN_ARGS names, none by default
make doc        # the module pages under build/doc/, and the manual pages under build/man/
make release    # with a release of ern and each file it carries committed: the
                # archive, build/<name>-<version>.tar.gz, and its checksum beside it
make install    # builds, then installs under PREFIX, /usr/local by default, from a
                # checkout or an unpacked archive: make install PREFIX=/home/me/opt/local
make uninstall  # removes from PREFIX what make install put there, then share/doc, share,
                # lib and bin under it, each where it is empty, and nothing else
```

A package the program loads is an entry of `package.conf`, its name, version, URL and digest, as the report's §11.9 says. `make lib` runs `ern unpack`, which unpacks each package from its archive under `lib/`, `lib/<package>-<version>.tar.gz`, and says which archive to download where one is not there; it then builds each Erlang application `ERL_DEPS` names, a git submodule under `erl/`, by its own `make`. `make` builds each package before the program.

Everything the program loads beyond the standard library and Ernest's own libraries is a package under `lib/` or an Erlang application under `erl/`, whose `ebin` `--libs-dir erl` puts on the load path of the tests and of the launcher, where there is one. A repository with an `erl/` is cloned with `--recursive`. A program of `examples/` is run with one argument, `build/examples/<program>` followed by the Makefile's `EXAMPLE_SUFFIX`, the path it writes. `make doc` writes the module pages, CommonMark, under `build/doc/`, and the manual pages, roff, under `build/man/`; a library's archive carries the module pages under `docs/modules/` and the manual pages under `docs/man/man3/`, which `man -M` reads. `make format` lays the modules out. `make clean` removes what the build wrote and each package `ern unpack` wrote beside its archive, and leaves the archives, a link under `lib/` and what each Erlang application built.

## Running

`bin/<name> [--config-dir dir] [argument]...` runs the program from the checkout and from an unpacked release alike, with the packages its `package.conf` names on the load path, and its Erlang; it runs the `ern` on `PATH`, or the one `ERN` names, and an `ern` before 0.11.0 answers that `--package-dir` is not an option of `ern run`. Once `make install` has put it under a prefix, the installed `<name>` runs the same way, by its path or by a link to it, with the packages under its own `lib/`. An installed program runs under the `ern` that built it, and once that `ern` changes, `make install` from the program's archive builds it again. `--config-dir dir` makes the run a node, as *Running Ernest*, the deployment guide of the installation, says; everything else goes to the program.

## The documents

`src/<name>.ern` is the entry module, or a library's root module, and [`docs/design.md`](docs/design.md) the program's design; in the repository, `docs/README.md` says what each other document is.

The tests live in the modules they test, which `make test` runs; `test/`, where it exists, holds tests run end to end, modules of tests that run the program with the checkout as their working directory, and `tools/` the checker of the documents; `make test` runs them too.

`make test` reads the project's history by its own forms, and lets a bare word through. A comment names no milestone, step or item followed by a number, whatever it counts; no finding by its name after the word "finding"; neither the plan's file nor the findings'; and no date written year, month and day. It may cite a log entry by its title, `the log's *Title*`. A line of this README, of `CHANGES.md` or of a module under `src/` names no milestone, step or item followed by a number. In the repository, `docs/release.md` gives a release's note its rules, the lines of `CHANGES.md` under a heading such as `## 1.2.0, 2026-11-23`; `make test` refuses there a date outside the heading, a finding, either file, a log entry, and a cold, code, document, independent or security reader.

## License

NAME is released under the Zero-Clause BSD license, 0BSD, the terms in [`LICENSE`](LICENSE). Third-party code, where there is any, is listed with its licenses in `THIRD_PARTY_LICENSES`.

## Beginning from the template

Make a repository from the template, *Use this template* on GitHub, or a clone with its `.git` removed and `git init` run in it, and then (`template/design.md` says why the template is as it is, and `template/log.md` how it came to be):

1. Set the Makefile's `NAME` to the program's name, one lowercase word or words joined by `_`; replace `NAME` and `<name>` with it in `CLAUDE.md` and this file; and rename `bin/name` and `src/name.ern` to it. A library has no launcher, and removes `bin/name`, *Running*, and the `make run`, `make install` and `make uninstall` lines.
2. Write `src/<name>.ern`, the module `Name`, with its first test: a program's `main` is its entry point, and a library's module exports what it offers. Every module stands at `src/<name>.ern` or under `src/<name>/`, so that the archive can be a dependency, as `docs/build.md` says. A test cites the design's section it holds in the comment above it, `// design §1: …`, and every section is cited.
3. Say what the program does above and in `docs/design.md`, and begin `docs/plan.md`; `docs/log.md`'s first entry names the template's tag, the newest under *Tags* on its GitHub page, which the files `CLAUDE.md` calls the template's are refreshed from.
4. Set `LICENSE`, 0BSD as the template has it, with its year and holder, or another, with the README's sentence to match; `VERSION`; and the entries of `package.conf` and the Makefile's `ERL_DEPS` as the program needs them. An Erlang application is a submodule under `erl/` of the application's name, read-only and pinned, never a copy, and only the application of the program's name carries a `priv/`: another is a package of its own. `THIRD_PARTY_LICENSES` appears with the first borrowed file, and `ACKNOWLEDGMENTS.md` with the first name.
5. Turn on private vulnerability reporting in the repository's settings, where `SECURITY.md` sends a reporter, and name the repository in `.github/ISSUE_TEMPLATE/config.yml`, which sends a security hole there.
6. Remove this section, the quoted line under the epigraph, `template/`, the template's own design note and log, its own issue form, `.github/ISSUE_TEMPLATE/rule.yml`, and its own `findings.md` and `language_feedback.md` under `docs/`, where they stand; and replace the two pictures under `assets/` with the program's own, uploading its social preview in the repository's settings. Then `git add -A` and `make test`, which reads the files git tracks; until this section and `template/` are gone, it names the paths the first step renamed.
