# Falke Security Research

Minimal Jekyll blog for red team and cybersecurity write-ups, built for [GitHub Pages](https://pages.github.com/).

Live URL (after Pages is enabled): **https://crpr777.github.io/Falke-Security-Research/**

Topics:

- Covert Methods of Entry
- Red Team Operations
- AI Security Research

There are no analytics or third-party trackers. New posts are Markdown files in `_posts/`.

## Write a new post

1. Copy `_templates/post.md` to `_posts/YYYY-MM-DD-short-slug.md`.
2. Set front matter:
   - `title` — page heading
   - `date` — used for sorting and the URL (`/:year/:month/:day/:title/`)
   - `categories` — exactly one of:
     - `Covert Methods of Entry`
     - `Red Team Operations`
     - `AI Security Research`
     (those strings must match so the [archive](archive.md) groups the post)
   - `tags` — free-form labels for the home list
   - `summary` — optional one- or two-sentence blurb on the home page; if omitted, Jekyll uses the excerpt
3. Write the body in Markdown (GitHub Flavored). Use fenced code blocks for highlighting.
4. Commit and push to `main`. GitHub Actions builds and deploys the site.

Placeholder posts in `_posts/` are templates only. Replace or delete them before publishing real work.

## Run locally

Requires Ruby 3+ and Bundler.

```bash
gem install bundler
bundle install
bundle exec jekyll serve
```

Open http://127.0.0.1:4000/Falke-Security-Research/ — `baseurl` is `/Falke-Security-Research` so local paths match the project site.

Build only:

```bash
bundle exec jekyll build
```

Output is `_site/`.

## Enable GitHub Pages

This repo deploys with GitHub Actions (`.github/workflows/pages.yml`), not the classic “branch /docs” publisher.

After this branch is merged to `main`:

1. Repo **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **GitHub Actions**.
3. If the workflow has not run yet, open the **Actions** tab and run **Deploy Jekyll site to Pages**, or push an empty commit to `main`.
4. The first deploy creates a `github-pages` environment. Approve it if the org requires environment protection.
5. Wait for the workflow to go green. The site is served at `https://crpr777.github.io/Falke-Security-Research/`.

`url` and `baseurl` in `_config.yml` are already set for that project-site address. If you later move this to a user site (`https://crpr777.github.io/`), set `baseurl` to `""`.
