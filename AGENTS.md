# PROJECT KNOWLEDGE BASE

**Generated:** 2025-12-30T22:20:00Z
**Commit:** 1c80c05
**Branch:** main

## OVERVIEW

LaTeX-based resume repository. Automated build workflow using TinyTeX via `mise` and VS Code LaTeX Workshop.

## STRUCTURE

```
curriculum-vitae/
├── .vscode/    # IDE settings (formatting, auto-build)
├── dist/       # Final published PDF artifacts
├── src/        # Source documents
│   ├── cv.latest.tex  # Primary source (entry point)
│   └── cv.v0.pdf      # Legacy reference
└── mise.toml   # Tool management & build tasks
```

## WHERE TO LOOK

| Task         | Location                | Notes                     |
| ------------ | ----------------------- | ------------------------- |
| Edit Content | `src/cv.latest.tex`     | Principal source file     |
| Build Task   | `mise.toml`             | Tasks: `build`, `dist`, `dev` |
| IDE Logic    | `.vscode/settings.json` | Formatter & Recipe config |

## CODE MAP

### Custom LaTeX Commands (Resume Framework)

| Symbol                       | Type    | Location            | Role                        |
| ---------------------------- | ------- | ------------------- | --------------------------- |
| `\resumeItem`                | Command | `src/cv.latest.tex` | Achievement bullet point    |
| `\resumeSubheading`          | Command | `src/cv.latest.tex` | Role/Company entry (2-line) |
| `\resumeItemListStart`       | Command | `src/cv.latest.tex` | Standard bullet list init   |
| `\resumeSubHeadingListStart` | Command | `src/cv.latest.tex` | Unlabeled list for roles    |

## CONVENTIONS

- **No Top-Level Bullets**: Experience roles must use `resumeSubHeadingListStart` with `label={}`.
- **Header Style**: Header links (`mailto`, `linkedin`, `github`) use `\href` without `\underline`.
- **Build Output**: Compilation artifacts redirected to `out/` via VS Code settings.

## ANTI-PATTERNS (THIS PROJECT)

- **Manual `dist/` edits**: Always generate `dist/` files via `mise run dist`.
- **Type Suppression**: Do not use `as any` or `@ts-ignore` (though primarily a TeX project).
- **Bullet in Job Title**: Never use `\resumeSubheading` inside a bulleted list; use `resumeSubHeadingListStart`.

## UNIQUE STYLES

- **Telegraphic Resume Style**: Sacrifice full sentences for impact-driven bullet points.
- **TinyTeX dependency**: Project strictly relies on TinyTeX distribution managed by `mise`.

## COMMANDS

```bash
mise run build  # Compile src/cv.latest.tex to out/
mise run dist   # Build and publish to dist/Brandon_Thenaro_CV.pdf
mise run dev    # Continuous build (watch mode)
```

## NOTES

- **README.md**: Symbolic link to `AGENTS.md`.
- **Formatter**: `latexindent` configured in VS Code settings.
