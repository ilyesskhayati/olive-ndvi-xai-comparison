# olive-ndvi-xai-comparison

Do different model classes explain the same wavelet-decomposed NDVI signal the
same way? XGBoost, Random Forest and Ridge regression are fitted to identical
inputs at a delineated olive orchard in Jendouba, Tunisia, and their feature
attributions compared.

Companion to `olive-ndvi-wavelet-xai`, which reproduces the framework this work
builds on. That repository is frozen; this one is not a reproduction.

## Study area

`olive-jendouba-polygon.geojson` — 0.644 km², delineated by hand on
high-resolution imagery where the olive planting grid is visible. About 10 MODIS
NDVI pixels at 250 m, and 0.64 of one MODIS LST pixel at 1 km.

## Notebooks

01  data acquisition        polygon extraction, spatial means
02  wavelet decomposition   discrete Meyer at native cadence
03  feature derivation      every predictor justified from evidence
04  model training          XGBoost, Random Forest, Ridge
05  attribution             SHAP and permutation, compared across models
06  selection               stratified, and Ridge as a neutral selector

## Setup

Uses the virtual environment from `olive-ndvi-wavelet-xai`. Select the
`olive-venv` kernel.