# Sigmoid Functions Explorer

A tiny, front-end–only web app to help students understand how the parameters a (slope) and b (intercept) affect:

- The line y = a x + b
- The logistic sigmoid σ(a x + b) = 1 / (1 + e^{-(a x + b)})

Two charts are shown side-by-side. Use the sliders to change a and b and see both plots update in real time.

## How to run

Open `index.html` in any modern browser. No build step or server required.

Optional: if you want to serve it locally to avoid CORS/file URL quirks on some setups, run a simple static server in this folder and open the provided URL.

## Files

- `index.html` – The single-page app using Chart.js via CDN.

## Notes

- Domain for x is [-10, 10] with step 0.05.
- Sliders: a ∈ [-5, 5], b ∈ [-10, 10].
- The sigmoid implementation uses a numerically stable form to avoid overflow for large |a x + b|.