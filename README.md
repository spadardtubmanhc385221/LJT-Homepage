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

## Deployment

The workflow builds and validates both pages, verifies that each contains all six publication titles, and publishes the generated static files to the `gh-pages` deployment branch. That branch is generated output; edit the source files on `master` instead.

GitHub Pages must also be enabled for the repository. Its automatic creation was blocked by the Actions integration's permissions during setup. In **Settings > Pages**, select **Deploy from a branch**, branch **gh-pages**, and **/(root)**, then save. The configured production URL is `https://spadardtubmanhc385221.github.io/LJT-Homepage/`. Until Pages is enabled, the workflow warns that live-site verification is skipped; a successful build does not mean the public URL is live. Once enabled, the workflow also checks both public URLs.

The original theme license is retained in `LICENSE`.
