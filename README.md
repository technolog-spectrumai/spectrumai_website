# Spectrum AI next-level Hugo patch

This patch replaces the old Tailwind/Alpine/tsparticles layout with a custom CSS Hugo layout inspired by the premium single-page style used in the reference site, but with a distinct Spectrum AI identity: operational intelligence, autonomy, agents, and decision infrastructure.

## Files included

```text
layouts/_default/spectrum.html
content/en/index.md
content/pl/index.md
content/fr/index.md
i18n/en.yaml
i18n/pl.yaml
i18n/fr.yaml
static/img/spectrum-mark.svg
static/_redirects
hugo.toml
netlify.toml
```

## Apply

From your Hugo project root:

```bash
unzip spectrum_nextlevel_patch.zip
cp -r spectrum_nextlevel_patch/* .
rm -rf public resources
hugo server -D --disableFastRender
```

Open:

```text
http://localhost:1313/en/
http://localhost:1313/pl/
http://localhost:1313/fr/
```

## Netlify

```bash
git add .
git commit -m "Add next-level Spectrum AI Hugo design"
git push
```

Netlify settings:

```text
Build command: hugo --minify
Publish directory: public
```
