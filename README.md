# CV 1050: Vector Calculus and Numerical Methods
## Interactive JupyterBook — Module 1: Vectors and Tensors

**Department of Civil Engineering, IIT Madras**

---

## Setup Instructions

### Prerequisites

```bash
pip install jupyter-book jupyterlab numpy matplotlib scipy ipywidgets
```

### Build and serve the book

```bash
# Build HTML
jupyter-book build cv1050_jupyterbook/

# View in browser — open cv1050_jupyterbook/_build/html/index.html
# Or serve locally:
python -m http.server 8000 --directory cv1050_jupyterbook/_build/html
# Then navigate to http://localhost:8000
```

### Run notebooks interactively (with widgets)

```bash
cd cv1050_jupyterbook
jupyter lab
```

Widgets (sliders) require the notebook to be **executed** in JupyterLab or Jupyter Notebook.
The built HTML (JupyterBook) shows static outputs; for interactive figures launch JupyterLab.

---

## Book Structure

| File | Topic | Lecture pages |
|------|-------|--------------|
| `notebooks/00_intro.ipynb` | Introduction and course map | — |
| `notebooks/01_geometrical_preliminaries.ipynb` | Geometrical objects & vectors | 2–4 |
| `notebooks/02_vector_operations.ipynb` | Addition, subtraction, scaling | 5–9 |
| `notebooks/03_dot_and_cross_products.ipynb` | Dot product, cross product, triples | 10–16 |
| `notebooks/04_index_notation.ipynb` | Index notation, δ_ij, ε_ijk | 17–24 |
| `notebooks/05_matrices_and_transformations.ipynb` | Matrices, rotations, coord. transforms | 25–49 |
| `notebooks/06_tensors.ipynb` | Second-order tensors: algebra & operations | 50–65 |
| `notebooks/07_eigenvalues_and_invariants.ipynb` | Eigenvalues, spectral decomp., invariants | 66–71 |

---

## Interactive Features per Chapter

| Chapter | Widgets | Code cells |
|---------|---------|------------|
| 1 | 3D vector + component bar chart | Rotation verification |
| 2 | 2D vector addition (head-to-tail + parallelogram) | Linear combination solver |
| 3 | Dot product + projection; 3D cross product + area | Vector identity verifier |
| 4 | δ_ij and ε_ijk heatmaps | Einstein summation with numpy.einsum |
| 5 | 2D coordinate rotation widget | Stress tensor transformation |
| 6 | Symmetric/skew decomposition heatmaps; tensor action in 3D | Traction vector, norm checks |
| 7 | Eigenvector 3D viewer; characteristic polynomial plotter | Principal stress analyser |

---

## Pedagogical Design

### AI-resistant assessment strategy
- All **self-check exercises** require **handwritten derivation first**
- Tutorial submissions are **in-person, handwritten**
- Code cells serve as **verification**, not derivation
- Questions are **parameterised** (different numbers per student) to prevent copying

### AI-assisted learning (encouraged)
- Use AI to **understand** what a code cell does
- Ask AI to **explain** why `np.linalg.norm(ch_check)` should be near zero
- Do **not** use AI to generate your homework solutions

---

## References

1. **Lecture slides**: CV 1050, Dept. of Civil Engineering, IIT Madras (2024–25)
2. **Saravanan, U. & Srinivas, C. A.**: *Tensor Algebra and Calculus*, IIT Madras, July 2024
3. **Hjelmstad, K. D.**: *Fundamentals of Structural Mechanics*, Springer — Ch. 1: Vectors and Tensors
