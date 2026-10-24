# LJT-Homepage

Personal academic website for Junteng Liu, based on [Academic Pages](https://github.com/academicpages/academicpages.github.io).

## Site content

- **About** (`/`): profile, research focus and interests, academic background, research experience, all six publications, honors, and contact details.
- **Publications** (`/publications/`): the same six publications, with full author lists, publication years, venues, and supplied authorship roles.

Only the supplied profile information is used. No unprovided portrait, CV download, paper link, or exact publication date is added. The research areas are used for the research-skills section; no technical-skills list was supplied separately.

## Content files and local preview

- `_pages/about.md`: the About page, including its publication list.
- `_publications/`: six publication records in the supplied order. Only publication years are stored; the collection does not generate individual paper pages.
- `_config.yml` and `_data/authors.yml`: identity and contact settings.
- `_data/navigation.yml`: the two navigation links.

Keep the About publication list and publication records in sync when editing.

```sh
bundle install
bundle exec jekyll serve
```

The production URL and `/LJT-Homepage` base path are configured in `_config.yml`. The deployment workflow builds the site and verifies that both pages contain all six publication titles.

The original theme license is retained in `LICENSE`.
