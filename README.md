# alessandrociardo.github.io

Personal academic website of Alessandro Ciardo — PhD candidate in Economics at the University of
Barcelona and the Barcelona Institute of Economics (IEB).

Built with [Jekyll](https://jekyllrb.com) on the
[Academic Pages](https://github.com/academicpages/academicpages.github.io) template and served by
GitHub Pages. Every push to `master` rebuilds the live site at
<https://alessandrociardo.github.io>.

## How to update the site

Everything that changes regularly lives in a handful of files. No Jekyll knowledge needed.

| What you want to change | File to edit |
| --- | --- |
| Front page text, job market blurb, references | `_pages/about.md` |
| A paper (title, coauthors, abstract, PDF link) | the matching file in `_publications/` |
| Add a new paper | new `.md` file in `_publications/` (copy an existing one) |
| Teaching | files in `_teaching/` |
| CV page | `_pages/cv.md` |
| Name, email, affiliation, social links, avatar | `_config.yml` (the `author:` block) |
| Menu items | `_data/navigation.yml` |
| Colours and fonts | `_sass/theme/_ciardo_light.scss` and `_ciardo_dark.scss` |
| Everything else about the styling | `_sass/_custom.scss` |

### Papers

Each paper is one Markdown file in `_publications/`. The front matter controls how it appears:

```yaml
---
title: "Paper title"
collection: publications
category: wip          # jmp | articles | wp | wip — see publication_category in _config.yml
permalink: /research/paper-slug
date: 2026-09-01       # controls the order within a section (most recent first)
coauthors: "with A. Coauthor and B. Coauthor"   # leave "" if sole-authored
status: ""             # optional line under the title, e.g. "Revise and resubmit, JUE"
draft_status: "Draft available upon request"    # shown when there is no paperurl
paperurl: '/files/paper-slug.pdf'               # add once the draft is public
slidesurl: '/files/paper-slug-slides.pdf'       # optional
excerpt: "One sentence used for search engines and link previews."
---

The abstract goes here, as normal text.
```

The `/research/` page groups papers into the sections listed under `publication_category` in
`_config.yml`, in that order. An empty section is skipped automatically.

### Job market banner

`_config.yml` has:

```yaml
on_the_market            : true
job_market_year          : "2026/27"
```

Set `on_the_market: false` to remove the banner from the front page once the season is over.

### PDFs

Put PDFs (CV, drafts, slides) in `files/`. They are served at
`https://alessandrociardo.github.io/files/filename.pdf`. The CV download button is commented out
near the top of `_pages/cv.md` — uncomment it once `files/cv-alessandro-ciardo.pdf` exists.

## Running the site locally (optional)

Not required — GitHub Pages builds the site on every push — but useful for previewing bigger changes.

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

Then open <http://localhost:4000>. Changes to Markdown and HTML refresh automatically; changes to
`_config.yml` need a restart.

## Credits

Template: [Academic Pages](https://github.com/academicpages/academicpages.github.io), a fork of the
[Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) Jekyll theme by Michael Rose,
released under the MIT License (see `LICENSE.md`).
