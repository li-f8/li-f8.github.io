# li-f8.github.io

Personal academic website of Fuwen Li — built with [Jekyll](https://jekyllrb.com) on the
[Academic Pages](https://github.com/academicpages/academicpages.github.io) template and
served by GitHub Pages at <https://li-f8.github.io>.

## Bilingual content (English / 中文)

The site renders both languages into every page and shows one at a time; the visitor
switches with the **中文 / EN** button in the header. English is what first-time
visitors see regardless of their browser locale; a choice made with the button is
remembered in `localStorage`.

To write bilingual content, wrap each language in a `div` (block) or `span` (inline):

```markdown
<div class="i18n-en" markdown="1">
English text here.
</div>

<div class="i18n-zh" markdown="1">
中文内容写在这里。
</div>
```

- `markdown="1"` is what lets Markdown work inside the `div` — don't drop it.
- Page titles in front matter take the same spans; add a plain `seo_title:` alongside
  them so the browser tab and social previews stay single-language.
- Strings that come from the theme rather than a page (footer, sidebar labels) live in
  `_data/i18n.yml` and are rendered with `{% include t.html key="..." %}`.

The mechanics are in `_includes/head/custom.html` (CSS + the pre-paint language choice)
and `_includes/footer/custom.html` (the toggle handler).

## Where things live

| What | Where |
| --- | --- |
| Site settings, sidebar profile, social links | `_config.yml` |
| Header menu | `_data/navigation.yml` |
| Home / About | `_pages/about.md` |
| Research | `_pages/research.md` |
| CV | `_pages/cv.md` |
| Publications page (currently off the menu) | `_pages/publications.html` |
| PDFs and other downloads | `files/` |
| Profile photo and images | `images/` |

## Adding a publication

1. Copy `_publications/_example.md` to `_publications/YYYY-MM-DD-paper-slug.md` and fill
   in the front matter (files starting with `_` are ignored by Jekyll, so the example
   itself never publishes).
2. Uncomment the Publications entry in `_data/navigation.yml`.

The CV page picks up publications automatically once the collection is non-empty.

## Running it locally

```bash
bundle install          # once
bundle exec jekyll serve -l -H localhost
```

Then open <http://localhost:4000>. Pushing to `master` republishes the live site.
