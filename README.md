# digitech — archived template customization

> **Provenance note (please read first).** This repository is an **archived snapshot**, not an
> original creation. It is a customization of the **Laralink "DigiTech"** commercial HTML template
> and was forked from [`Sharoonss/digitech`](https://github.com/Sharoonss/digitech). The visual
> design, layout, and the bulk of the markup/CSS/JS belong to the upstream template author
> (**Laralink**). It is preserved here for archival and reference purposes only and is **kept
> private**. See [`NOTICE`](./NOTICE) for the trademark/copyright statement.

## What this is

A static, multi-page marketing site for a digital-agency brand ("DigiTech"), built on the Laralink
DigiTech HTML template and adapted for a business contact (`digitechtrading.net`). It ships as plain
HTML/CSS/JS — no build step, no framework.

Pages included:

- `index.html` — home
- `about/about.html` — about
- `Services/services.html` — services overview
- `service detail*/detail*.html` — individual service pages
- `blog/blog.html` — blog listing
- `contact/contact.html` — contact form

## What was changed for this archived copy

To keep the archived snapshot clean and safe to store, the following edits were made to the
imported template. **No authorship is claimed over the underlying template.**

- **Removed portrait photos of people** — the template's team-member and testimonial headshots
  (`images/member_*.jpeg`, `images/testimonial_*.jpeg`) were deleted and replaced with a neutral
  placeholder avatar (`images/avatar-placeholder.svg`).
- **Redacted a form key** — the live [Web3Forms](https://web3forms.com) `access_key` on the contact
  form was replaced with the placeholder `YOUR_WEB3FORMS_ACCESS_KEY`. Supply your own key to make the
  form functional.

## Running it locally

No dependencies, no build. Just serve the folder over HTTP so the relative links resolve:

```bash
# from the repo root
python3 -m http.server 4933
# then open http://localhost:4933/index.html
```

Any static file server works (`npx serve`, VS Code Live Server, etc.). Opening `index.html` directly
via `file://` mostly works too, though root-relative paths (`/images/...`) resolve best over HTTP.

## Credits

- **Template:** "DigiTech" by **Laralink** (`meta author` in every page).
- **Upstream repository:** [`Sharoonss/digitech`](https://github.com/Sharoonss/digitech).

This snapshot is not affiliated with, endorsed by, or a product of Laralink. All template rights
remain with their respective owners.
