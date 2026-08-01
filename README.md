# abirami.github.io

Personal site, served by GitHub Pages. One file, no build step, no framework.

## Publishing checklist

1. Repository must be named exactly `<your-username>.github.io` and be **public**.
2. `index.html` sits at the root of the `main` branch.
3. Settings &rarr; Pages &rarr; Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
4. First build takes 1-2 minutes. The site is then live at `https://<your-username>.github.io`.

## Placeholders to replace

Search `index.html` for these and swap in the real values:

| Placeholder | Where it appears |
|---|---|
| `YOUR-GITHUB-USERNAME` | rail link + all five project links |
| `YOUR-LINKEDIN` | rail link |
| `YOUR-EMAIL` | rail link and the contact section |

## Adding a photo

Create an `images/` folder, drop in `profile.jpg` (square, roughly 400x400), then in `index.html`
replace the monogram div with:

```html
<img class="monogram" src="images/profile.jpg" alt="Abirami Senthilkumar">
```

## Editing

- Project entries live in `<section id="projects">`. Copy one `<li class="check">` block to add another.
- Roles live in `<section id="experience">`, same pattern with `<li class="role-item">`.
- Colours and fonts are CSS custom properties at the top of the `<style>` block.

## Checking a change before pushing

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```
