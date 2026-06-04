# Yidan Sun Personal Website

This repository powers [yidans.github.io](https://yidans.github.io/). It is a Jekyll site based on AcademicPages and is deployed by GitHub Pages from the `master` branch.

## Main Content Files

- `_pages/about.md` - homepage biography and news
- `_pages/publications.md` - research page, publications, manuscripts, and presentations
- `_pages/cv.md` - CV page
- `_pages/portfolio.md` - gallery page
- `_data/navigation.yml` - top navigation
- `_config.yml` - site metadata, author profile, and Jekyll settings
- `images/` - profile and gallery images

## Local Preview

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

Then open <http://localhost:4000>.

## Updating Content

1. Add new news items at the top of `_pages/about.md`.
2. Add accepted or published work to `_pages/publications.md`, grouped by year.
3. Move manuscripts out of "Preprints and Manuscripts" after they are published.
4. Put new gallery images in `images/` and add a new `<figure>` block to `_pages/portfolio.md`.
5. Run `bundle exec jekyll build` before pushing.

## File Organization Notes

The repository intentionally keeps the AcademicPages theme files under `_includes`, `_layouts`, `_sass`, and `assets`. Demo posts, sample talks, sample publications, and sample teaching pages should stay out of the repo unless they are real site content.
