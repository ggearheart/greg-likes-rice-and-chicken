# Greg Likes Rice & Chicken 🍚🐔

**A World Atlas of the Planet's Favorite Pairing** — an open-source cookbook and
website of iconic chicken-and-rice dishes from around the world, built with
[Quarto](https://quarto.org).

It's two things at once:

- a **browsable website** (the rendered Quarto book), and
- a downloadable **book** in PDF and EPUB, from the same source.

## The dishes

| Dish | Home | Technique |
|---|---|---|
| Hainanese Chicken Rice | 🇸🇬 Singapore | Poach & serve |
| Oyakodon | 🇯🇵 Japan | Simmer over rice |
| Arroz Caldo | 🇵🇭 Philippines | Congee / porridge |
| Hyderabadi Chicken Biryani | 🇮🇳 India | Layered *dum* pilaf |
| Zereshk Polo ba Morgh | 🇮🇷 Iran | Steamed pilaf + tahdig |
| Chicken Kabsa | 🇸🇦 Saudi Arabia | One-pot pilaf |
| Jollof Rice | 🇳🇬 West Africa | One-pot pilaf |
| Arroz con Pollo | 🇪🇸 Spain / Latin America | One-pot pilaf |
| Chicken Jambalaya | 🇺🇸 Louisiana, USA | One-pot Creole/Cajun |
| Trinidad Pelau | 🇹🇹 Trinidad & Tobago | Caramelized one-pot |

Plus **Foundations** chapters: why the pairing works, Rice 101, and a cook's
toolkit of shared techniques.

## Build it yourself

You need [Quarto](https://quarto.org/docs/get-started/) installed.

```bash
# live preview with hot reload (opens in your browser)
quarto preview

# render the website + PDF + EPUB into _book/
quarto render

# render just the website
quarto render --to html
```

> **PDF note:** the PDF format needs a LaTeX toolchain. The easiest route is
> `quarto install tinytex` (a self-contained, no-sudo LaTeX install).

The rendered site lands in `_book/`.

## Project layout

```
_quarto.yml            # book config: chapters, formats, theme
index.qmd              # the landing / welcome page
chapters/              # one .qmd per chapter (foundations + 10 dishes)
assets/                # SCSS themes, cover + favicon (SVG)
references.bib         # sources for the histories
references.qmd         # bibliography + further reading
.github/workflows/     # auto-deploy to GitHub Pages
```

## Contributing

Corrections, regional variations, and whole new dishes are all welcome — see
[chapters/contributing.qmd](chapters/contributing.qmd). The short version: copy an
existing chapter, follow the recipe format, register it in `_quarto.yml`, and open
a pull request.

## License

- **Content** (text, recipes, images): [CC BY-SA 4.0](LICENSE-CONTENT)
- **Code** (SCSS, config, workflows): [MIT](LICENSE-CODE)
