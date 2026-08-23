# ML Algorithms — Interactive Visualizer

A single-file, landscape (16:9) slide deck that explains **Regression** and
**Classification**, then walks through 13 algorithms — each with a **live,
interactive visualizer** (drag sliders, click the plot to add data points).

## Contents (17 slides)

1. Title
2. Regression — definition & when to use
3. Classification — definition & when to use
4. **Linear Regression** — least-squares line, residuals, R²
5. **Polynomial Regression** — degree slider, overfitting
6. **Decision Tree Regression** — depth slider, step function
7. **Random Forest Regression** — number of trees, smoothing
8. **Support Vector Regression** — ε-insensitive tube
9. **Ridge Regression** — L2 shrinkage (coefficient bars)
10. **Lasso Regression** — L1 sparsity (coefficients → 0)
11. **Logistic Regression** — sigmoid decision boundary
12. **Decision Tree Classifier** — axis-aligned regions
13. **Random Forest Classifier** — ensemble vote regions
14. **K-Nearest Neighbors** — k slider, voting regions
15. **Support Vector Machine** — linear / RBF kernel, margins
16. **Naive Bayes** — Gaussian likelihood regions
17. Summary — how to choose

## Controls

- **← / →** (or PageUp/PageDown / Space) — previous / next slide
- **F** — toggle fullscreen
- **Home / End** — first / last slide
- Sliders & buttons under each plot — change model parameters live
- **Click the plot** — add a data point and watch the model refit

No build step, no dependencies — everything is vanilla JS/Canvas in `index.html`.

## Publishing to GitHub Pages

**Option A — serve from repo root**

1. Copy `index.html` to the root of the repo you'll publish (or move this folder's file there).
2. Push to GitHub.
3. Repo → **Settings → Pages** → *Build and deployment* → **Deploy from a branch** → branch `main`, folder `/ (root)` → **Save**.
4. Your deck goes live at `https://<username>.github.io/<repo>/`.

**Option B — serve this subfolder**

1. Keep `index.html` inside `ml-visualizer/`.
2. In **Settings → Pages**, choose branch `main` and folder `/ (root)`.
3. Open `https://<username>.github.io/<repo>/ml-visualizer/`.

> Tip: GitHub Pages needs an `index.html` — this file is already named correctly.
