# Linear Regression — Pizza Price Prediction

A beginner-friendly machine learning project that demonstrates **simple linear regression** by predicting pizza prices from diameter using [scikit-learn](https://scikit-learn.org/).

---

## Overview

The model is trained on a small dataset mapping pizza diameter (inches) to price (USD). Given a new diameter, it extrapolates the expected price using a fitted linear regression line.

| Diameter (in) | Price (USD) |
|:---:|:---:|
| 8 | $10 |
| 10 | $13 |
| 12 | $16 |

**Example prediction:** a 20-inch pizza → **$28.00**

---

## Prerequisites

- Python 3.8+
- [pip](https://pip.pypa.io/en/stable/)
- [Jupyter Notebook](https://jupyter.org/) or [JupyterLab](https://jupyterlab.readthedocs.io/)

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/sharad-bista/linear-regression.git
cd linear-regression
```

### 2. Create and activate a virtual environment

```bash
python -m venv venv

# macOS / Linux
source venv/bin/activate

# Windows (PowerShell)
.\venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch the notebook

```bash
cd pizza_prediction
jupyter notebook pizza.ipynb
```

Run all cells with **Kernel → Restart & Run All** (or `Shift+Enter` cell by cell).

---

## Project Structure

```
linear-regression/
├── pizza_prediction/
│   └── pizza.ipynb        # Jupyter notebook — data, model, prediction
├── requirements.txt       # Python dependencies
├── .gitignore
├── LICENSE
└── README.md
```

---

## How It Works

1. **Data** — three (diameter, price) pairs are defined as NumPy arrays.
2. **Training** — `sklearn.linear_model.LinearRegression` fits a line through the points.
3. **Prediction** — the fitted model predicts the price for an unseen diameter.

The relationship learned is:

```
price = slope × diameter + intercept
```

Because the data is perfectly collinear the model achieves an R² of 1.0 on the training set.

---

## Dependencies

| Package | Purpose |
|---|---|
| `numpy` | Numerical arrays |
| `scikit-learn` | Linear regression model |
| `jupyter` | Interactive notebook environment |

See [requirements.txt](requirements.txt) for pinned versions.

---

## License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.
