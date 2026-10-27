# NAME

*The Importance of Being Ernest, a Trivial Comedy for Serious People*

What the program does, in a paragraph. This repository was begun from [`ernest-template`](https://github.com/joagre/ernest-template), whose last section says how.

## Building

It needs [Ernest](https://github.com/joagre/ernest) on your `PATH`, the floor the Makefile names, `ern 0.6`; `make` says so where another is found. `ERN=path/to/ern make` names another `ern`.

```
make            builds: lib/ filled, each dependency and then the program compiled
make test       the layout, every module's tests, the documents and the design's citations,
                listing without failing any paragraph past about a hundred words,
                test/ and examples/ where they exist
make run        runs the program through its launcher, bin/NAME
make release    the archive, build/NAME-VERSION.tar.gz
make man        a library's manual pages into docs/man/, committed with its release
```

`make lib` fills `lib/` with each dependency `DEPS` names by the URL of its release archive, fetched and unpacked once, and each Erlang application `ERL_DEPS` names, a git submodule under `erl/` built by its own `make` and linked.

Everything the program loads beyond the standard library and Ernest's own libraries stands under `lib/`: a dependency's `build`, on the load path by `--load-path`, and an Erlang application's `ebin`, on it by `--libs-dir lib`. A repository with an `erl/` is cloned with `--recursive`. `make doc` writes each module's documentation under `build/`, `make format` lays the modules out, and `make clean` removes what the build and `make lib` wrote.

## Running

`bin/<name> [--config-dir dir] [argument]...` runs the program from the checkout and from an unpacked release alike, with everything under `lib/` on the load path. `--config-dir dir` makes the run a node, as *Running Ernest*, the deployment guide of the installation, says; everything else goes to the program.

## The documents

- [`docs/design.md`](docs/design.md): how the program is arranged, the normative document of this repository, and the glossary of its names.
- [`docs/plan.md`](docs/plan.md): where the program stands and what comes next.
- [`docs/log.md`](docs/log.md): the dated rationale, never normative.
- [`docs/release.md`](docs/release.md): what a release runs to be ready.
- `docs/proposals/`: what is designed, a directory for each proposal, from the first one on.
- `language_feedback.md`, from its first line: what writing Ernest felt against the principles, carried to Ernest by copy.
- [`CLAUDE.md`](CLAUDE.md): the working rules.

The tests live in the modules they test, which `make test` runs; `test/`, where it exists, holds a program run end to end, and `tools/` the checker of the documents, `make test` runs them too.

## License

NAME is released under the Zero-Clause BSD license, 0BSD, the terms in [`LICENSE`](LICENSE). Third-party code, where there is any, is listed with its licenses in `THIRD_PARTY_LICENSES`.

## Beginning from the template

Make a repository from the template, *Use this template* on GitHub or a clone with its `.git` removed, and then (`TEMPLATE.md` says why the template is as it is):

1. Replace `NAME` in `Makefile`, `CLAUDE.md` and this file with the program's name, one lowercase word or words joined by `_`, and rename `bin/name` to it; a library has no launcher, and removes it.
2. Write `src/<name>.ern`, the module `Name` whose `main` is the entry point, with its first test, and `make test`.
3. Say what the program does above and in `docs/design.md`, and begin `docs/plan.md`'s first milestone; `docs/log.md`'s first entry names the template's tag, which `tools/docs.ern` is refreshed from.
4. Set `LICENSE`, 0BSD as the template has it or another, with the README's sentence to match, `VERSION` and the Makefile's `DEPS` and `ERL_DEPS` as the program needs them, an Erlang application as a submodule under `erl/`, read-only and pinned, never a copy; `THIRD_PARTY_LICENSES` appears with the first borrowed file, and `ACKNOWLEDGMENTS.md` with the first name.
5. Remove this section and `TEMPLATE.md`, the template's own design note.
