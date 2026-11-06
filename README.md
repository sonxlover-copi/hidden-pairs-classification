# Hidden Pairs Classification

A reproducible tabular classification workflow for the Hidden Pairs assignment. It validates the supplied CSV schemas, trains a baseline, compares a small set of classical models, and writes a submission file.

## What it covers

- Input schema and row-count checks
- A decision-tree baseline and ROC-AUC evaluation on the validation set
- Comparison of compact scikit-learn models
- Selection using validation data and export of test predictions

## Data

The course data is not stored in this repository. Obtain `week-03-hidden-pairs.zip` from the course materials and extract it into `data/datasets/hidden-pairs/` beside the notebook. The folder should contain `train.csv`, `validation.csv`, `test.csv`, and `sample_submission.csv`. Do not commit the dataset or generated submission.

## Run locally

Python 3.10 or newer is recommended. Create an environment and install the dependencies:

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
python -m pip install -r requirements.txt
jupyter lab
```

Open `hidden_pairs.ipynb` and run all cells. It writes `submission.csv` to the notebook's working directory.

## Validation

The recorded run passed the schema checks, reached validation ROC-AUC 0.7473 with the baseline tree, and generated 1,116 test predictions.

## Attribution

This is an adapted solution to an educational laboratory. The original assignment and its course attribution are preserved in the notebook.
