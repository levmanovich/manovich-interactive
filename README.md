# ImagePlot 2

**Interactive visualization of image collections.**  
Single self-contained HTML file — open in any browser, no installation required.

---

## What it does

ImagePlot 2 automatically extracts **48 visual features** from a set of images — brightness, saturation, hue, entropy, contrast, and others — and plots your collection as an interactive scatter visualization, with images rendered directly as data points.

Key capabilities:

- **Scatter plot** with any two features on X and Y axes
- **PCA and t-SNE** to visualize the full high-dimensional feature space in 2D
- **Compare mode** to overlay two collections and see their footprints side by side
- **Animate images in feature space** — for example, using dates on X shows changes in images' visual features over time
- **Hover and zoom** — click any image to inspect it; scroll to zoom, drag to pan
- **Save view** — export any visualization as a PNG

---

## What it is for

ImagePlot 2 is a tool for **cultural analytics** and **art historical research** — for anyone who works with large image collections and wants to explore patterns that are invisible to the naked eye.

The underlying idea is that of a **style space**: a 2D projection of quantified visual properties of images, where position encodes visual similarity. Images that are visually alike cluster together; images that differ stand apart. By choosing which features to plot, you can explore different dimensions of style, composition, or color — and follow how they evolve over time.

---

## Included sample collections

Two sample datasets are included to get started:

- **Van Gogh paintings** — 360 images (199 Paris, 161 Arles) created when the artist lived in Paris and Arles, and corresponding metadata files with dates and titles; can be used to compare the two periods in style space.
- **Mondrian paintings** — 128 images (1905–1917), with corresponding metadata file containing dates.

---

## Example uses (using included datasets)

### Van Gogh: Paris vs. Arles

Plotting 199 Paris paintings (1886–1888) and 161 Arles paintings (1888) on brightness (X) and saturation (Y) axes reveals the differences and similarities in van Gogh's paintings between the two periods in relation to brightness and saturation. The Arles cluster sits higher and to the right — brighter, more saturated — but the two clouds overlap significantly, showing that stylistic change was gradual rather than sudden. You can apply the same approach to any image set, or place two sets together in the same feature space to compare their visual footprints.

### Mondrian: evolution over time

Compute all 48 features for 128 Mondrian paintings (1905–1917), project them into 2D using t-SNE, then play the animation with image ID on the X axis. This traces the trajectory of Mondrian's work through feature space in chronological order, making gradual stylistic shifts visible as movement across the plot.

### Mondrian: color groups

Plotting the same paintings with brightness mean on X and hue median on Y reveals a clear division into two groups: paintings dominated by brown and red tones cluster at the bottom, while paintings dominated by blue and violet tones cluster at the top. A single feature combination makes visible a color structure that spans the entire period.

---

## How to use

1. Open `imageplot_2.html` in any modern browser
2. Load a collection using the **Load Images** button (folder of JPEGs or PNGs)
3. Optionally load a metadata TSV file to add dates and any other information to be used in the visualizations
4. Choose X and Y axes from the 48 extracted features, or switch to PCA / t-SNE
5. Explore, zoom, compare, save

See `imageplot2_guide.html` for full step-by-step instructions.

**Performance note:** The tool has been tested with collections of up to ~1,000 images without noticeable slowdown. With larger collections, behavior may be unpredictable — the tool will run increasingly slowly or may quit.

---

## Background

ImagePlot 2 is a browser-based reimagining of the original **ImagePlot** software developed by the [Software Studies Initiative](http://lab.culturalanalytics.info) (2009–2011). The original tool, built in ImageJ, enabled the large-scale image visualizations that became foundational examples of cultural analytics. ImagePlot 2 is adding many new features, and is easy to customize — just open the file in any AI coding assistant and ask it to add new features, change the UI, and so on.

The theoretical framework behind this approach — style space, visual footprints, and the analysis of image collections over time — is developed in:

> Lev Manovich. **"Style Space: How to Compare Image Sets and Follow Their Evolution."** Draft, August 2011. Included in this repository as `style_space_2011.pdf`.

> Lev Manovich. **Cultural Analytics.** The MIT Press, 2020. Contains detailed theoretical analysis of the ImagePlot method and related visualization methods for exploring image collections.

For dozens of examples of cultural analytics projects applying image visualization to datasets ranging from art history to manga to media — see the [Cultural Analytics Lab](http://lab.culturalanalytics.info).

---

## Credits

ImagePlot 2 — Lev Manovich, 2024–2025.  
Original ImagePlot — Lev Manovich, Jeremy Douglass, Nadia Xiangfei Zeng, Software Studies Initiative, 2009–2011.

Part of [manovich-interactive](https://github.com/manovich/manovich-interactive).
