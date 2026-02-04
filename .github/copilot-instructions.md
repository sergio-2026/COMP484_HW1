# Copilot instructions — COMP484_HW1

Purpose
- This is a small static website for COMP 484 (homework 1). Pages are plain HTML with a single stylesheet in `_css/styles.css` and images in `images/`. Primary pages: [index.html](index.html), [links.html](links.html), [next.html](next.html), [reference.html](reference.html), [structure.html](structure.html), [syntax.html](syntax.html). Tasks in `lab_instructions.txt` drive content/format changes.

Big picture
- No backend or build tooling: files live in the repo root and are served directly by a web server or opened in a browser.
- Styles are centralized in [_css/styles.css](_css/styles.css). HTML pages reference that stylesheet and use classes like `flowRight` / `flowLeft` for image layout — do not remove those class names when editing markup.

Developer workflows
- Preview locally: run `python -m http.server 8000` from the repo root and open `http://localhost:8000`.
- In VS Code, using the Live Server extension is acceptable for rapid previews.
- There are no automated tests or build steps. Editing is done directly in the HTML/CSS files.

Project-specific conventions & patterns
- Pages live at repository root and are linked with relative URLs. Preserve relative link structure when renaming or moving files.
- Use the existing CSS classes and folder structure: `_css/` for styles and `images/` for media. Filenames are lowercase and use no spaces.
- Follow the assignment-driven content patterns in [lab_instructions.txt](lab_instructions.txt): headings across pages should be consistent; `next.html` expects specific line-break and emphasis changes; `reference.html` contains an entity table that must use HTML entities.
- Note: `lab_instructions.txt` contains a few typographical mistakes (for example it mentions `index.htmll` and `reference.htm`); rely on actual filenames in the repository when making edits.

Concrete examples to follow
- Heading strategy: inspect [index.html](index.html) and the other pages named above and apply consistent heading levels across pages (see step 1 in [lab_instructions.txt](lab_instructions.txt)).
- Emphasis/line breaks: for `next.html`, move the opening sentence of each recommendation to its own line and emphasize per instructions in `lab_instructions.txt`.
- Images: when inserting the W3C logo on `index.html`, point to `images/200px-W3C_icon.png`, set `alt="W3C logo"`, `width="200"`, `height="136"`, and add class `flowLeft` (assignment step 6).

Integration points & external deps
- None required. The site targets any modern browser. Use a simple static server for previews.

Notes for an AI coding agent
- Prefer minimal, focused edits: change only the files and lines required by the lab tasks.
- Preserve formatting and CSS class names; do not refactor global structure unless the user asks.
- When the instructions reference a page that doesn't match an exact filename in the repo, prefer the actual filename present in the workspace.
- When adding markup examples, keep them valid HTML and avoid adding external dependencies.

If any section above is unclear or you want the file structured differently, tell me which part to expand or change.
