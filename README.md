# Lab: NumPy Jupyter Notebooks

This repository contains a set of Jupyter notebooks and supporting files used in a NumPy / linear algebra lab.

## Contents

- Jupyter notebooks (.ipynb) covering NumPy basics and linear algebra exercises.
- `quiz.py`, `utils.py` and some helper images in the `images/` folder.

Files you may see in the root:

- `C1_W1_Lab_1_introduction_to_numpy_arrays.ipynb` — Introduction to NumPy arrays
- `C1_W1_Lab_2_linear_systems_as_matrices.ipynb` — Linear systems as matrices
- `C1W3_UGL_1_vector_operations.ipynb` — Vector operations (current working notebook)
- `test_numpy.ipynb` — Small notebook for quick testing
- `quiz.py`, `utils.py` — helper scripts

## Requirements

- Python 3.8+ (recommended 3.8–3.11)
- Jupyter Notebook / JupyterLab
- NumPy

Install common dependencies with pip:

```powershell
python -m pip install --upgrade pip
python -m pip install jupyter numpy
```

If you're using a virtual environment (recommended):

```powershell
python -m venv .venv; .\.venv\Scripts\Activate.ps1; python -m pip install -U pip jupyter numpy
```

## How to run

Start Jupyter in the repository root and open the notebook you want:

```powershell
jupyter notebook
```

Each notebook contains explanatory text and code cells. Run cells with Shift+Enter.

## Quick push to GitHub (PowerShell)

If you want to push this repository to GitHub, from the repository root run:

```powershell
git init
git add .
git commit -m "Add lab notebooks and resources"
git branch -M main
git remote add origin https://github.com/<your-username>/Lab-numby-jupyter.git
git push -u origin main
```

Replace `<your-username>` with your GitHub username and ensure the remote repo exists (or create it on github.com).

## Notes

- Notebooks may include outputs or cached files. Consider cleaning outputs before committing large results.
- This README is intentionally concise. Add more project-specific instructions if you plan to share this repo.

---

Created: October 4, 2025
