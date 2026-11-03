# Forest Cover Type: from raw data to predictions

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/El-Moghazy2/space-apps-2026-forest-cover/blob/main/forest_cover_colab.ipynb)

A standalone notebook for the **AI & Machine Learning workshop at NASA Space Apps Cairo 2026**, built on Kaggle's [Forest Cover Type Prediction](https://www.kaggle.com/c/forest-cover-type-prediction) competition.

**The task:** predict which of 7 tree cover types grows on a 30 m × 30 m cell of forest in northern Colorado, using only map measurements: elevation, slope, distances to water, roads and fire points, soil type.

| Step | What it covers |
|---|---|
| 1 | Load the data (downloads automatically, no Kaggle account needed) |
| 2 | Feature dictionary: what every column means, including the decoded soil codes |
| 3 | First look: size, quality, class balance |
| 4 | Exploration: what separates the cover types |
| 5 | Feature engineering |
| 6 | A test set of unseen forest areas (why random rows flatter the model) |
| 7 | Extra trees: training and evaluation |
| 8 | Which features the model uses |
| 9 | Final model, correcting for the real forest's class mix, and `submission.csv` |

**Run it:** click the badge, then *Runtime → Run all*. It needs only the libraries Colab already has, and runs in a few minutes.

## Data

Blackard, J. A. & Dean, D. J., Colorado State University. UCI Machine Learning Repository, [Covertype](https://doi.org/10.24432/C50K5N), CC BY 4.0. Features come from US Geological Survey and US Forest Service maps; labels from US Forest Service surveys. Kaggle's `train.csv` is the first 15,120 rows of this file and `test.csv` the rest.
