# Dataset Setup

This folder is reserved for the datasets used in the COMP813 project, **Cross-Dataset Generalisation of NLP Models for Phishing Email Detection**.

The project uses the following datasets:

## 1. Enron Email Dataset

The Enron dataset is used to train and evaluate the email classification models.

- **Purpose:** Model training and in-dataset evaluation.
- **Used by:** TF-IDF with Logistic Regression, TF-IDF with linear SVM, and BiLSTM.
- **Setup:** Obtain the dataset from its authorised source and place the required data files in this folder, following the filenames and format expected by the notebooks.

## 2. CEAS-08 Dataset

The CEAS-08 dataset is used for external evaluation to investigate how well models generalise to a different email dataset.

- **Purpose:** Cross-dataset evaluation and analysis.
- **Used for:** Performance comparison, domain-shift analysis, error analysis, sequence-length ablation, and robustness experiments.
- **Setup:** Obtain the dataset from its authorised source and place the required data files in this folder, following the filenames and format expected by the notebooks.

## Expected Folder Structure

The exact filenames may vary depending on the dataset versions and preprocessing used.

```text
data/
├── README.md
├── enron.csv       # Example filename only
└── ceas08.csv      # Example filename only
```

The example filenames above are placeholders. Use the actual filenames expected by the project notebooks.

## Important Notes

- The datasets are not included in this repository.
- Users must obtain the datasets from their authorised sources and comply with the applicable licence, privacy, and usage requirements.
- Do not upload raw email data containing personal or sensitive information unless redistribution is explicitly permitted.
- Configure the dataset paths in the notebooks to match the local file locations.
- Dataset versions, preprocessing steps, column names, and label mappings must remain consistent with the experimental setup documented in the project report.

## Reproducibility

Before running the notebooks, ensure that both datasets are available locally and that the required columns and label formats match the preprocessing code. Run the notebooks in the documented order and refer to the project README for environment setup and execution instructions.
