# Haar Cascade Face and Eye Detection

An OpenCV notebook for inspecting classic face and eye detection across example photos. It uses cascade classifiers bundled with OpenCV and draws detection rectangles over the images.

[Open the notebook](haar-face-eye-detection.ipynb)

## Run locally

From the repository root, use a fresh Python 3.11 environment.

```bash
python -m pip install -r requirements.txt
python -m jupyterlab
```

Place your own shareable photos named `face2.jpg`, `side.jpg`, and `side2.webp` beside the notebook, then run its cells in order.

## What to compare

The notebook converts input images to grayscale and searches for structures at multiple scales with `detectMultiScale`. Inspect the annotated outputs across front-facing and angled examples. Compare missed or extra boxes as pose and lighting change.

These cascades demonstrate detection of image regions. The notebook does not identify people or report a benchmark on a labeled face dataset.
