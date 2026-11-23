# Known issues

What is known to be wrong or missing and not planned, a line each, until the user takes one up.

- **`tools/docs.ern` reads Markdown by its own rules.** A lone backtick pairs with the next one as a span, and a fence of four backticks ends at a line of three inside it, so a path or a paragraph after either can be passed over. It waits for Ernest's `Markdown.parse` to give each block its line, a line of `language_feedback.md`.
