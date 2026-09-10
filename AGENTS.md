# Agent Guidelines for Academic Pages (academicpages.github.io, v.0.9.x)

**This file contains important information for coding agents working in this repo.**

`academicpages.github.io` is a Jekyll theme for academic, professional, and personal portfolio-oriented websites. The the typical use pattern is to "Use this template" to "Create a new repository" (see [Creating a repository from a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) where the user will make their own edits to customize the template to create their own personal GitHub pages website. 

If a user has created a personal website, there is **no need** to create a pull request back to the `academicpages.github.io` repository.

## This site's conventions

This repository is a personal website built from the template, not the template itself.

- **Bilingual content.** Every page carries English and Chinese; only one is visible at a
  time. Wrap block content in `<div class="i18n-en" markdown="1">` / `<div class="i18n-zh"
  markdown="1">` and inline content in the matching `<span>`. Never add content in one
  language only — add both, or ask.
- Front-matter titles use the same spans and pair with a plain `seo_title:`.
- Theme strings (footer, sidebar) go in `_data/i18n.yml`, rendered via `_includes/t.html`.
- The language toggle lives in `_includes/masthead.html`, with its CSS and pre-paint
  script in `_includes/head/custom.html` and its handler in `_includes/footer/custom.html`.
