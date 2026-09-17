# LibreKO website

The source of [libreko.org](https://libreko.org) — a single static page, no build step and no
dependencies.

```
index.html    the page
styles.css    tokens + layout
```

Open `index.html` in a browser, or serve the folder:

```
python -m http.server 8000
```

Deploy by copying both files to any static host.

## Editing

- **Design tokens** (colour, type, spacing) are CSS custom properties at the top of `styles.css`.
- **Repository links** are the `#repos` table in `index.html`; the clone and Docker commands sit in
  the `#get` section, each with a `data-copy` attribute that the copy button reads.
- **The test client download** is the button in `#get`; update its `href` when a new build is uploaded.
- **Fonts** come from Google Fonts. Self-host them if you would rather the site made no third-party
  requests.

## Licence

AGPL-3.0, like the rest of LibreKO. See [LICENSE](LICENSE).
