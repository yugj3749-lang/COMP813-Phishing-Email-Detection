# Environment and Dependencies

## Python environment

Use Python 3.10 or 3.11 in a virtual environment where possible. The notebooks use
the packages listed in `requirements.txt`.

## Install dependencies

From the repository root, run:

```bash
python -m venv .venv
```

Activate the environment:

**Windows (PowerShell)**
```powershell
.venv\\Scripts\\Activate.ps1
```

**macOS / Linux**
```bash
source .venv/bin/activate
```

Then install the project dependencies:

```bash
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

PyTorch installation can depend on the operating system and whether GPU support is
needed. If the default installation does not suit your machine, follow the official
PyTorch installation selector: https://pytorch.org/get-started/locally/

## Main dependencies

- **pandas, NumPy:** loading and manipulating datasets and numerical operations.
- **scikit-learn:** TF-IDF vectorisation, Logistic Regression, Linear SVM, and
  evaluation metrics.
- **PyTorch:** BiLSTM model implementation and inference.
- **Matplotlib, Seaborn:** plots and visual analysis.
- **SciPy:** statistical testing in the error analysis.
- **joblib:** saving and loading fitted models and related artefacts.

Python standard-library modules such as `os`, `re`, `json`, `time`, and
`collections` are also used; they do not need to be installed separately.

## Reproducibility note

The project notebooks and saved classical models have previously shown a
scikit-learn version mismatch (the model was created with scikit-learn 1.7.2
and loaded with 1.6.1). Loading persisted scikit-learn estimators across
versions can produce warnings or inconsistent behaviour.

For a reproducible run, use the same scikit-learn version for training and
evaluation, and ideally retrain and evaluate the models within the same
environment. Record the actual versions used for the final experiments. The
requirements file lists minimum versions and is not a lockfile, so it does not
guarantee an identical environment across machines.

To record the environment after installation, run:

```bash
python --version
python -m pip freeze
```

If exact versions are required for marking, save the output of `python -m pip freeze`
as a separate environment record after confirming that the notebooks run correctly.
