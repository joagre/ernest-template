# Language feedback

What writing Ernest felt against the principles, a line each, carried to Ernest as `CLAUDE.md`'s *The work* says. These come from the template's full review at `d8b7ab4` and its round over the fixes, with `ern 0.11.0+93a13b13`; each names its finding in the readers' lists, which the findings held at `c9bc7c1`. They were carried by message, and close by message.

- **`Markdown.parse` gives no block its line** (C47). A tool that reports a file and a line cannot use Ernest's CommonMark reader, so `tools/docs.ern` reads Markdown itself, and what it reads wrong is a line of `known_issues.md` meanwhile (C13). Principle 2. Ask: each block's line, counted from 1; the checker then reads by `Markdown.parse`. Held by Ernest's plan, its feedback 320.
- **`unknown name List.each` offers no near name** (the round's K18). `List.forEach` stands in the same module. Principle 3. Ask: the help names the nearest name the module exports. Held by Ernest's plan, its feedback 289.
