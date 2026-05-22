# CLAUDE.md — intro-stats

Notes for Claude Code (or any AI assistant) working in this repo.

## What this repo is

A **public-facing course resource site** for Matt Hester's Intro to
Statistics course. It is a sibling of the main site at
[matthewhester.com](https://matthewhester.com) and will eventually
live at `/intro-stats/` under that domain.

This is **not** a raw course archive. The LMS still owns dates,
rosters, grades, and full syllabi. This site holds curated, sanitized,
public-safe material: conceptual notes, generic activity descriptions,
small example datasets, and external resource pointers.

## Privacy and publication rules

**Do not publish:**

- Student data (any kind: identifiable, deidentified, or aggregated
  from a small section).
- Class rosters, grade distributions, or anything pulled from the LMS.
- Internal school documents (committee notes, internal policy memos,
  emails, accreditation materials).
- FERPA-adjacent material — work samples that came from identifiable
  students, recorded class sessions, gradebook screenshots, etc.
- Verbatim institutional policy text. Summarize and link instead.

**Be careful with:**

- Material copied wholesale from the school archive. Do **not** bulk-
  import; curate piece by piece and sanitize each one.
- Datasets that "feel public" but were actually shared under a use
  agreement.
- Old slide decks with embedded student names, photos, or work.

When unsure, default to **don't publish** and ask. It is much easier to
add material than to retract it from a public site.

## Design intent

- Loose visual match to the main site — same stone/iron palette, same
  restraint. Do not introduce new accent colors.
- Quarto sidebar/book-like structure. Navbar carries top-level
  sections (Home / Syllabus / Schedule); sidebar carries the deeper
  navigation (Notes / Activities / Assignments / Projects / Resources).
- Plain CSS, no JS, no SCSS pipeline.

## Editing rules

- Top-level pages: `index.qmd`, `syllabus.qmd`, `schedule.qmd`.
  Section landing pages: `notes/index.qmd`, `activities/index.qmd`,
  `assignments/index.qmd`, `projects/index.qmd`, `resources/index.qmd`.
- Each section will grow into multiple sibling `.qmd` files; add new
  files in the matching directory and update the sidebar in
  `_quarto.yml`.
- Datasets live in `data/`; supporting figures in `assets/`.
- `_site_planning/` is local-only — excluded from render and not part
  of the public site.

## Build

- `quarto render` from repo root.
- Output goes to `_site/` (gitignored).
- No CI yet. This is local-only until the main site goes live.
