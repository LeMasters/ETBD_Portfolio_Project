# ETBD Portfolio Project

Documents for faculty in Emerging Technology in Business and Design (Miami University) about how undergraduate games students build and present professional portfolios: what we ask of a portfolio, how we review one quickly, and the department platform students publish on.

Most of what is here is narrative: instructions, explanations and the reasoning behind them. The platform itself lives elsewhere (see "Related repositories").

## What's here

| Folder | Contents | Read it if you want to… |
| --- | --- | --- |
| [`portfolio-reviews/`](portfolio-reviews/) | The ten review guidelines (five on what a portfolio must communicate, five on how studios filter portfolios), and two earlier handouts as PDFs | Understand what we look for, or run a fast review |
| [`student-materials/`](student-materials/) | What students receive: setup instructions, best practices, a blank **portfolio worksheet**, and short guides on Hugo, search engines and AI, domain names, and first-portfolio habits | See exactly what students are told, or hand a guide to a student |
| [`faculty/`](faculty/) | The instructor setup guide: the platform's current state, setup steps, a verification checklist, troubleshooting, lessons learned and the roadmap | Set up or support the platform for a class |
| [`sample-personas/`](sample-personas/) | Three fictional students (Robert Herrick, John Donne, Anne Southwell), the method used to build them, and the worksheets their sample sites were filled from | See finished examples, or compare how one student's material supports different portfolio "arguments" |

### The portfolio worksheet

[`student-materials/portfolio-worksheet.md`](student-materials/portfolio-worksheet.md) is a blank worksheet a student fills in before opening the site editor. Its sections follow the template's eight forms, in order and with the same labels (Profile, Selected Work, Gallery, Experience, Education, Tools, Appearance, Analytics). It carries a version line and a change log; version 1.3 matches Alexander 0.6.6. The three filled examples are in [`sample-personas/worksheets/`](sample-personas/worksheets/).

## The platform in one paragraph

Students copy a department template, **Alexander** (a Hugo theme), into their own GitHub account. They edit it through web forms in **Pages CMS**; each save triggers a GitHub Actions build that publishes the site on **GitHub Pages**. No code and nothing to install. The content is stored as plain Markdown and YAML files, one per project, job or degree, so it can outlive any particular design. Details and reasoning: [`faculty/instructor-setup-guide.md`](faculty/instructor-setup-guide.md).

## Related repositories

| Repository | What it is |
| --- | --- |
| [`LeMasters/portfolio_template_Alexander`](https://github.com/LeMasters/portfolio_template_Alexander) | The template students copy. Its `docs/DESIGN.md` explains how the theme works and why |
| [`portfolio_RobertHerrick`](https://lemasters.github.io/portfolio_RobertHerrick/), [`portfolio_JohnDonne`](https://lemasters.github.io/portfolio_JohnDonne/), [`portfolio_AnneSouthwell`](https://lemasters.github.io/portfolio_AnneSouthwell/) | The three sample sites (links go to the live sites), built from the template and filled through Pages CMS |

## About these copies

The student guides and the worksheet are edited as Claude Docs; the files here are Markdown copies of them, made 23 November 2026 for Alexander 0.6.6. When a guide changes, update its copy here too. The persona dossiers mention placeholder-image folders and working notes that are not in this repository.

Not included: working notes for the AI assistant that helped build the platform, and the calibration review of a real student's portfolio (it concerns an actual student).

Garrison LeMasters · Department of Emerging Technology in Business and Design, College of Creative Arts, Miami University
