# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **creative-writing project**, not a software application. It contains
only UTF-8 Markdown files (Chinese-language 商周祭祀文化 × 玄幻修仙 worldbuilding and
manuscript) under `firstnovel/`. There is **no build system, dependency manifest, lint
config, test suite, or runnable service**.

- There is nothing to install, compile, lint, test, or serve. Do not attempt to detect or
  create a package manager (npm/pip/etc.) — there is none, and one should not be added
  unless the user explicitly asks.
- The startup update script is intentionally a no-op (`true`); no dependency refresh is
  needed for prose files.
- The "product" is the manuscript itself. To review content, read the Markdown directly.
  If a rendered preview is useful, render with any Markdown tool of your choice into a temp
  directory (e.g. `pip install --user markdown` then a short render script) and serve it —
  but keep such tooling out of the repo and out of the update script.
- Authoring workflow is governed by `firstnovel/novelrules.md`. Before writing or editing
  any prose/settings, read `novelrules.md` first, then the relevant canon files in
  `firstnovel/worlddesign/00`–`12` per the reading-order table in that file. Content
  conflicts are resolved by the priority list in `novelrules.md` (theme/`00` > mechanics
  `01` > characters `06`/`07` > world `02`/`04` > presentation `05` > chapter outline `09`
  > macro plan `08` > style sample `10` > progress log `03`).
- Filenames contain CJK characters; always quote paths in shell commands.
