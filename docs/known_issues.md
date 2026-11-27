# Known issues

What is known to be wrong or missing and not planned, a line each, until the user takes one up.

- **`tools/docs.ern` reads Markdown by its own rules, but for code spans and fences.** A backtick escaped by `\` still opens or closes a span, a span runs on into a heading or a list item that follows its line with no blank line between, a line that begins with three backticks and holds another opens a fence where CommonMark reads a span, and an indented code block is read as prose, so the checker can pass over a path or check one that is code. It waits for Ernest's `Markdown.parse` to give each block its line, a line of `language_feedback.md`.
