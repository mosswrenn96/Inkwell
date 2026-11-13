# Inkwell

**Type on real-looking paper.** Inkwell is a small browser app that makes typed text look handwritten in ink on textured paper. Pick a paper and a handwriting font, then start typing. You can export the page as an image or PDF, or cut out pieces with torn or scissor-cut edges to use in collages.

It's a single HTML file with no install, build step or account. Open it in a browser and start writing.

<!-- Add a screenshot: save one as screenshots/inkwell.png and uncomment the next line -->
<!-- ![Inkwell screenshot](screenshots/inkwell.png) -->

---

## Features

### Writing
- **Type like in a word processor.** Click the page and start typing. Text wraps inside adjustable page margins.
- **Movable text boxes.** Add as many as you like, then drag them by the "move" tab, resize them from the corner, or delete them.
- **Formatting:** font, size, bold, italic, underline, strikethrough, alignment (left, center, right, justify), line height and letter spacing.
  - With text selected, changes apply to the selection.
  - With nothing selected, changes apply to the whole page or the selected text box.
- **Ink colors:** blue-black, black, ballpoint blue, sepia, red and graphite, plus a custom color picker.

### Ink that looks real
Text blends into the paper (multiply blend) and is roughened by an adjustable ink filter:

| Setting | What it does |
|---|---|
| Roughness | Wobbly, irregular stroke edges |
| Bleed | Ink spreading slightly into the paper fibers (off by default) |
| Unevenness | Patchy ink density, as if the pen pressure varied |
| Grain | Scale of that patchiness, from broad pools of ink to a fine pencil-like texture |
| Opacity | Overall ink strength |

Presets: **Fountain pen, Ballpoint, Pencil, Felt marker, Clean.** If typing feels slow on an older computer, turn off **Live effect**. The effect is still applied when you export.

### Paper
- **8 starter papers**: Cream stationery, Bright cotton, Notebook (ruled), Legal pad, Graph paper, Kraft, Aged parchment and Recycled grey.
- **Paper tint:** recolor any paper with a swatch or a custom color.
  - Four blend modes: Tint (keeps the paper's texture), Deepen, Soft light and Overlay.
  - Strength is capped so the tint can't drown out the text, and ruled lines keep their own color.
- **Your own papers:** load any photo or scan (JPG, PNG, WebP) as a paper. It can be tinted too.
- **Page sizes:** Letter, A4, A5, Legal, Index card (6×4) and Square (1080 px, for social posts).

### Fonts
- **15 starter handwriting fonts** from Google Fonts: Caveat, Homemade Apple, La Belle Aurore, Dancing Script, Cedarville Cursive, Nothing You Could Do, Reenie Beanie, Indie Flower, Shadows Into Light, Patrick Hand, Kalam, Gochi Hand, Covered By Your Grace, Rock Salt, and Special Elite (typewriter).
- **Your own fonts:** load `.ttf`, `.otf`, `.woff` or `.woff2` files.

### Cut-outs for collages
Cut out any part of the page, with its paper and writing, as a transparent PNG.

1. Click **Cut out** (the scissors button).
2. Draw your selection in one of two modes:
   - **Freehand:** drag around the area and let go to finish.
   - **Points:** click to place corners, and drag for curved stretches. Finish by clicking the first point, double-clicking, pressing Enter or tapping **Done**.
3. Choose an edge:
   - **Scissor cut:** clean, with a slight hand-cut wobble.
   - **Torn:** an uneven edge with a light fibrous rim.
   - **Pinking:** a zig-zag edge, like pinking shears.
   - **Deckle:** the soft, feathered edge of handmade paper.
4. Optionally add a soft drop shadow, then **Copy image** or **Download PNG**. Cut-outs are saved at 2× resolution.

It works with a mouse, a finger or a stylus.

### Export
- **PNG, JPEG, WebP or PDF.**
- **Three quality levels:** Screen (1×), High (2×) and Print (300 dpi).
- **PDFs are image-only:** the text is not selectable or searchable.

### Projects
- **Save project** writes a `.inkwell.json` file with your text, text boxes, paper, tint, ink settings, and any fonts and papers you loaded. **Open project…** brings it all back.
- Your work also autosaves in the browser, so reopening the app picks up where you left off.

### Interface
- **Light, Dark or System theme.** Use the button at the top right. System follows your computer's setting.
- **Clean layout:** one formatting toolbar, plus a **Studio** side panel for ink, paper tint, margins, your library and projects.

---

## Getting started

**Use it locally:** download `index.html` and open it in your browser.

**Host it free with GitHub Pages:**
1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**. Select your main branch and the `/ (root)` folder.
4. After a minute your copy is live at `https://<your-username>.github.io/<repo-name>/`.

---

## Keyboard shortcuts

| Keys | Action |
|---|---|
| Ctrl/⌘ + B / I / U | Bold / italic / underline |
| Ctrl/⌘ + S | Save project |
| Enter | Finish the cut-out selection |
| Backspace / Delete | Undo the last cut-out point (while cutting) |
| Esc | Clear the selection; press again to leave the cut-out tool or close the preview |

---

## Tips

- **Ruled paper:** keep the line height at **32** (the ruled and legal papers set this automatically). Nudge the **Top** margin in Studio until the writing sits on the lines.
- **More realistic handwriting:** use a little roughness and unevenness with a slightly off-black ink. Blue-black and sepia look more natural than pure black.
- **Collages:** export or copy cut-outs with the shadow off if your collage app adds its own shadows.

---

## Browser support

Works best in **Chrome, Edge and Firefox** on desktop, tablet and phone.

- **Safari:** editing works, but exports may come out without the roughened ink texture, because Safari's canvas filter support is limited.
- **Copy image** needs clipboard permission. If the browser blocks it, use **Download PNG** instead.

---

## Known limitations

- **One page per project.** A warning appears if text runs past the bottom.
- **Starter fonts need an internet connection** because they load from Google Fonts. Fonts you load yourself work offline.
- **Text boxes can't be rotated yet.**

---

## Credits & licenses

- **Starter fonts:** from [Google Fonts](https://fonts.google.com/?category=Handwriting), licensed under the [SIL Open Font License](https://openfontlicense.org/) (Apache 2.0 for a few). They are loaded from Google, not bundled.
- **Starter papers:** generated by the app's own code, so no image files are included.
- **Other sources:** good places for more papers and fonts are [Poly Haven](https://polyhaven.com/textures) and [ambientCG](https://ambientcg.com) (CC0 textures), Unsplash and Pexels (free-to-use photos), and Google Fonts. Check each item's license before redistributing it in this repository.

## License

See [LICENSE](LICENSE).
