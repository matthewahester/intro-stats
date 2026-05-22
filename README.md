# intro-stats

Public-facing course resource site for **Intro to Statistics**, taught
by Matt Hester at UA Little Rock. Sibling to the main site
[matthewhester.com](https://matthewhester.com); eventually lives at
`/intro-stats/` under that domain.

This is a **curated public resource site**, not a raw course archive.
See [`CLAUDE.md`](CLAUDE.md) for what does and does not belong here.

## Local development

```bash
quarto render     # build to _site/
quarto preview    # live preview
```

## Layout

```
intro-stats/
├── _quarto.yml              # site config, navbar, sidebar
├── index.qmd                # landing page
├── syllabus.qmd             # public syllabus summary
├── schedule.qmd             # generic week-by-week topic map
├── notes/index.qmd          # lecture notes (section landing)
├── activities/index.qmd     # in-class activities
├── assignments/index.qmd    # public assignment descriptions
├── projects/index.qmd       # open-ended projects
├── resources/index.qmd      # readings, R primers, links
├── data/README.md           # small public datasets
├── assets/README.md         # figures and supporting files
├── styles.css               # stone-toned palette
├── CLAUDE.md                # privacy + editing rules
└── _site_planning/          # local-only planning (not published)
```

No CI, no deploy. Local builds only for now.
