# NAME

*The Importance of Being Ernest, a Trivial Comedy for Serious People*

What the program is, for its reader, then where to begin, in a paragraph, with no argument its documents make. This repository was begun from [`ernest-template`](https://github.com/joagre/ernest-template), whose last section says how.

## Building

It needs [Ernest](https://ernest-lang.org) on your `PATH`, the floor the Makefile names, `ern 0.10`; `make` says so where another is found. `ERN=path/to/ern make` names another `ern`: its directory stands first on `PATH` for everything the build starts, so whatever names `ern` by its name, a test or an example's shell, runs that one too. A file not called `ern` is not reached this way.

```
make            builds: lib/ filled, each dependency and then the program compiled
make test       the layout, every module's tests, test/ and the examples where they exist,
                then the documents and the design's citations,
                refusing any paragraph past 150 words and any comment or
                text a user reads that names the project's history
make examples   each program of examples/ built and run, what it writes under build/examples/
make run        runs the program through its launcher, bin/NAME
make release    the archive, build/NAME-VERSION.tar.gz, and its checksum beside it
make install    installs what stands built under PREFIX, /usr/local by default, from a
                checkout or an unpacked archive: make install PREFIX=/home/me/opt/local
make uninstall  removes from PREFIX what make install put there, then share/doc, share,
                lib and bin under it, each where it is empty, and nothing else
```

`make lib` fills `lib/` with each dependency `DEPS` names by the URL of its release archive, fetched and unpacked once, and each Erlang application `ERL_DEPS` names, a git submodule under `erl/` built by its own `make` and linked.

Everything the program loads beyond the standard library and Ernest's own libraries stands under `lib/`: a dependency's `build`, on the load path by `--load-path`, and an Erlang application's `ebin`, on it by `--libs-dir lib`. A repository with an `erl/` is cloned with `--recursive`. `make doc` writes each module's page under `build/`, and a library's archive carries the pages under `docs/man/`. `make format` lays the modules out, and `make clean` removes what the build and `make lib` wrote.

## Running

`bin/<name> [--config-dir dir] [argument]...` runs the program from the checkout and from an unpacked release alike, with everything under `lib/` on the load path. Once `make install` has put it under a prefix, the installed `<name>` runs the same way, with everything under its own `lib/` on the load path. `--config-dir dir` makes the run a node, as *Running Ernest*, the deployment guide of the installation, says; everything else goes to the program.

## The documents

`src/<name>.ern` is the entry module, and [`docs/design.md`](docs/design.md) the program's design; in the repository, `docs/README.md` says what each other document is.

The tests live in the modules they test, which `make test` runs; `test/`, where it exists, holds a program run end to end, and `tools/` the checker of the documents, `make test` runs them too.

## License

NAME is released under the Zero-Clause BSD license, 0BSD, the terms in [`LICENSE`](LICENSE). Third-party code, where there is any, is listed with its licenses in `THIRD_PARTY_LICENSES`.

## Beginning from the template

Make a repository from the template, *Use this template* on GitHub or a clone with its `.git` removed, and then (`TEMPLATE.md` says why the template is as it is, and `TEMPLATE_LOG.md` how it came to be):

1. Replace `NAME` in `Makefile`, `CLAUDE.md` and this file with the program's name, one lowercase word or words joined by `_`, and rename `bin/name` to it; a library has no launcher, and removes it.
2. Write `src/<name>.ern`, the module `Name` whose `main` is the entry point, with its first test, and `make test`.
3. Say what the program does above and in `docs/design.md`, and begin `docs/plan.md`; `docs/log.md`'s first entry names the template's tag, which the files `CLAUDE.md` calls the template's are refreshed from.
4. Set `LICENSE`, 0BSD as the template has it or another, with the README's sentence to match, `VERSION` and the Makefile's `DEPS` and `ERL_DEPS` as the program needs them, an Erlang application as a submodule under `erl/`, read-only and pinned, never a copy; `THIRD_PARTY_LICENSES` appears with the first borrowed file, and `ACKNOWLEDGMENTS.md` with the first name.
5. Turn on private vulnerability reporting in the repository's settings, where `SECURITY.md` sends a reporter, and name the repository in `.github/ISSUE_TEMPLATE/config.yml`, which sends a security hole there.
6. Remove this section, `TEMPLATE.md`, the template's own design note, and `TEMPLATE_LOG.md`, its log, and replace the two pictures under `assets/` with the program's own, uploading its social preview in the repository's settings.
