# Linear Algebra for Machine Learning — NumPy Jupyter Labs

This repository contains short, hands-on Jupyter notebooks designed to teach and practice core linear algebra concepts used in machine learning, implemented with NumPy. The materials are intended for self-study, classroom labs, or assignments.

## What you'll learn

- Represent vectors and matrices with NumPy
- Perform vector and matrix arithmetic (addition, scaling, dot products)
- Solve linear systems using matrix methods
- Understand matrix properties that matter in ML (rank, invertibility)
- Apply linear algebra primitives to simple ML tasks (projections, linear regression basics)

## Notebooks (quick overview)

Files in this repo (open the ones you need):

- `C1_W1_Lab_1_introduction_to_numpy_arrays.ipynb` — NumPy fundamentals: arrays, slicing, broadcasting, and performance tips.
- `C1_W1_Lab_2_linear_systems_as_matrices.ipynb` — Model linear systems as Ax = b, solve with `numpy.linalg.solve`, interpret solutions.
- `C1W2_Assignment.ipynb` — Assignment notebook with exercises and cells for your answers (submission-ready).
- `C1W3_UGL_1_vector_operations.ipynb` — Vector operations, norms, unit vectors, and geometric interpretation.
- `test_numpy.ipynb` — Small playground for trying NumPy snippets.

Other helper files (may or may not be present): `quiz.py`, `utils.py`, and an `images/` folder with explanatory diagrams.

If a notebook name in your copy differs slightly, open the .ipynb files in the repo root to see the content.

## Prerequisites

- Python 3.8 or newer (3.8–3.11 recommended)
- Jupyter Notebook or JupyterLab
- NumPy (latest stable release recommended)

On Windows PowerShell, install quickly:

```powershell
python -m pip install --upgrade pip
python -m pip install jupyter numpy
```

Using a virtual environment (recommended):

```powershell
python -m venv .venv; .\.venv\Scripts\Activate.ps1; python -m pip install -U pip jupyter numpy
```

## Open and run the notebooks

1. Start Jupyter from the repository root:

```powershell
jupyter notebook
```

2. Click a notebook to open. Read the explanatory Markdown cells, then run code cells with Shift+Enter.

3. Many notebooks include small exercises. For assignment notebooks (e.g. `C1W2_Assignment.ipynb`), there are dedicated answer cells — keep your solutions in those cells.

Tips for working with the notebooks:

- Restart the kernel and Run All cells if you want a clean run: Kernel -> Restart & Run All.
- Use small helper prints to inspect shapes: print(arr.shape) and dtype to avoid broadcasting mistakes.
- Save often (Jupyter does auto-save but commit to git before major changes).

## Suggested workflow for the assignment

1. Open `C1W2_Assignment.ipynb` and read the instructions.
2. Work through the supporting labs (`C1_W1_Lab_1...`, `C1_W1_Lab_2...`, `C1W3_UGL_1_vector_operations.ipynb`) to review concepts.
3. Implement answers directly in the assignment notebook cells.
4. When ready, export the assignment notebook as HTML or keep the .ipynb and push it to your repo for submission.

## Exercises & extensions (optional)

- Implement a simple linear regression using normal equations (X^T X) and compare with `numpy.linalg.lstsq`.
- Experiment with ill-conditioned matrices: generate matrices with nearly-dependent columns and observe solver behavior.
- Visualize vector projections in 2D using matplotlib (add `matplotlib` to requirements).

## Troubleshooting

- If you see shape errors, print shapes of operands and ensure compatible dimensions for matrix multiplication (`@` or `np.dot`).
- If `numpy.linalg.solve` raises a LinAlgError (singular matrix), check matrix rank with `np.linalg.matrix_rank(A)`.

## Contributing

If you have improvements or new exercises, please open a PR. Keep notebooks focused (small, clearly documented cells) and add tests where reasonable.

## License & attribution

These materials are provided for learning and classroom use. If you adapt or redistribute, cite the original author.

---

Created/updated: October 4, 2025

