# Rim Hajal — Academic Website

Personal academic website for Rim Hajal (PhD student), built with [Jekyll](https://jekyllrb.com/)
using a customized copy of the [Texture theme](https://github.com/samarsault/texture) by samarsault
(MIT licensed — see `LICENSE.txt`).

## Structure

```
_config.yml         # site settings: name, tagline, nav, social links, colors
_data/
  publications.yml  # edit this to add/remove publications — no HTML needed
_posts/              # news / research updates (blog-style homepage feed)
about.md            # bio / research interests
research.md         # research overview & current projects
publications.md     # renders _data/publications.yml
cv.md                # CV summary + link to a CV PDF
contact.md          # contact details
assets/cv/          # put your CV PDF here (see cv.md)
```

## Editing content

- **Site title, tagline, colors, nav, social links:** edit `_config.yml` (the `texture:` block).
- **About / Research / CV / Contact text:** edit the corresponding `.md` file directly — it's plain
  Markdown with a few `[bracketed placeholders]` to fill in.
- **Publications:** add entries to `_data/publications.yml`; the publications page updates automatically.
- **News / updates:** add a new file to `_posts/`, named `YYYY-MM-DD-title.markdown`, following the
  format of the existing example post.
- **Color scheme:** set `texture.style` in `_config.yml` to one of `yellow`, `red`, `black`, `blue`,
  `green`, `purple`.

## Running locally

Requires [Ruby](https://www.ruby-lang.org/) and [Bundler](https://bundler.io/).

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000 in your browser. The site will rebuild automatically as you edit files.

## Deploying to GitHub Pages

1. Push this repo to GitHub (e.g. `github.com/rimhajal/rimhajal.github.io` for a user site, or any
   repo name for a project site).
2. In the repo settings, under **Pages**, set the source to **GitHub Actions** (a workflow is already
   included at `.github/workflows/pages.yml`), *or* set it to build from the `main` branch if you
   prefer GitHub's default Jekyll build.
3. If you're deploying to `https://<username>.github.io/<repo-name>/` (a project site, not a user
   site), set `baseurl: "/<repo-name>"` in `_config.yml`. For a user site or a custom domain, leave
   `baseurl` empty.

## Credits

Theme: [Texture](https://github.com/samarsault/texture) by samarsault, MIT License.
