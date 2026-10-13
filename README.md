# 💖 DSCI100 Study Social: Midterm Review Deck

An easy-to-navigate **Quarto reveal.js slide deck** for the WiDS@UBC DSCI100 study social ✨
Every coding exercise runs **live in your browser** with [webR](https://docs.r-wasm.org/webr/latest/) 🧪, so there's nothing to install. Just open the slides and start coding!

---

## 🚀 Quick start

Serve the folder over HTTP (opening `index.html` by double-clicking may not work with webR 🙈):

```bash
# option 1: Python
python3 -m http.server 8000
# then open http://localhost:8000

# option 2: Quarto
quarto preview index.qmd
```

Or publish the whole folder to **GitHub Pages** 🌐 or **Quarto Pub** 📮.

> ⏳ **First load:** R and the tidyverse download into your browser, so give it 20-60 seconds. After that it's cached.

---

## 🗺️ What's inside (63 slides)

| # | Section | What you'll find |
|---|---------|------------------|
| 01 | 🧭 **Strategy** | Exam format, the formula sheet, anatomy of a function |
| 02 | 🧹 **Tidyverse functions** | `read_csv`, `filter`, `select`, `arrange`, `slice`, `map`, `mutate`, `group_by`, `summarize` |
| 03 | 🔮 **Questions & tidy data** | Types of questions and answers, tidy data, file paths |
| 04 | 📊 **Data visualization** | Choosing, refining and explaining plots |
| 05 | 🗄️ **Databases** | SQLite vs PostgreSQL, `tbl()` and `collect()` |
| 06 | 🎯 **Classification & K-NN** | How K-NN works, tidymodels, centering and scaling |
| 07 | 🌿 **Version control** | Git, GitHub, the four commands, merge conflicts |
| 08 | 🎀 **Wrap-up** | Practice hub, next steps, good luck |

---

## 🧪 Live coding exercises

Six exercises, each with starter code and a click-to-reveal solution:

1. 🏷️ **Question classification**: a matching quiz with a Check button
2. 🧼 **Filter, select, mutate, arrange, slice**: wrangle `iris`
3. 📐 **Group by and summarize**: mean sepal length per species
4. 🌈 **Visualization**: a colored scatter plot with labels
5. 🌸 **K-NN classification**: predict the species of a new iris
6. 🌱 **Version control**: define the Git commands

There are also little **"Try it"** cells sprinkled through the tidyverse slides.

---

## 🎬 Animations

Pure CSS, with a ↻ **Replay** button on each:

- 🔎 `filter()` and `select()`: rows and columns fade away
- 🗺️ `map_df()`: a function visits every column
- ✨ `mutate()`: a new column is born
- 🎯 **K-NN in action**: distances, the K nearest, a majority vote
- ⚖️ **Centering & scaling**: watch the nearest neighbour change

---

## ⌨️ Navigation tips

| Key | What it does |
|-----|--------------|
| ← → | Previous / next slide |
| `M` or ☰ | Slide menu with every slide listed 📋 |
| `Esc` or `O` | Overview grid 🔭 |
| `F` | Fullscreen 🖥️ |
| `?` | All keyboard shortcuts |

📜 Slides taller than the screen scroll with your mouse wheel, trackpad or touch. Reveal shortcuts pause while your cursor is inside a code editor, so click outside it to use the arrow keys again.

---

## 📁 Project structure

```
dsci100-study-deck/
├── index.qmd         ✍️  the deck's source (edit this!)
├── theme.scss        🎨  colors, fonts, cards, animations
├── header.html       🧩  favicon, background, replay + scroll script
├── _extensions/      🔌  the quarto-webr extension
├── img/              🖼️  logo, screenshots, favicon
├── index.html        📄  the rendered deck
└── index_files/      📦  libraries for the rendered deck
```

After editing, re-render with:

```bash
quarto render index.qmd
```

---

## 🎨 Make it yours

| I want to... | Edit... |
|--------------|---------|
| 🌈 Change colors | the hex codes in `theme.scss` |
| 🔤 Resize the code editors | `editor-font-scale` at the top of `index.qmd` |
| ⏱️ Speed up or slow down animations | the `animation:` lines in `theme.scss` |
| ➕ Add an exercise | copy a `{webr-r}` cell and its `<details class="solution">` block in `index.qmd` |

**Palette** 💅: navy `#0e2a47` · purple `#a152a8` · pink `#e8afc0` · mint `#aed8c8` · cream `#fff4be`
**Font:** Helvetica Bold

---

## 📝 Good to know

- 🌐 webR and the code editor load from a CDN, so you need an internet connection.
- 📦 **Exercise 5** has a one-time "Step 0" cell that installs `tidymodels` and `kknn` in your browser (about 1-2 minutes). Run it first and wait for it to finish.
- 🔢 The K-NN animation data (ages, incomes, points) is made up purely for illustration.

---

## 💌 Credits

Made with 💜 for **WiDS@UBC**'s DSCI100 Study Social.
Built with [Quarto](https://quarto.org/) and [quarto-webr](https://github.com/coatless/quarto-webr) by James Balamuta.

Good luck on your midterm. You've got this! 🌟
