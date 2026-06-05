# Machine Learning

A personal collection of machine learning projects built from the ground up, starting with the fundamentals.

---

## Linear Regression

Linear regression is one of the oldest and most widely used algorithms in statistics and machine learning. It models the relationship between one or more **input variables (features)** and a **continuous output variable (target)** by fitting a straight line — or a hyperplane in higher dimensions — through the data.

The equation for simple linear regression:

```
y = mx + b
```

Where:
- `y` — predicted output
- `x` — input feature
- `m` — slope (how much y changes per unit of x)
- `b` — intercept (value of y when x = 0)

For multiple features (multiple linear regression):

```
y = w₁x₁ + w₂x₂ + ... + wₙxₙ + b
```

The model learns the weights `w` and bias `b` by minimizing the **Mean Squared Error (MSE)** — the average squared difference between predicted and actual values.

---

## Why Linear Regression in ML?

| Reason | Detail |
|---|---|
| **Interpretability** | Coefficients directly show the impact of each feature on the output — easy to explain to non-technical stakeholders |
| **Speed** | Training is near-instant even on large datasets; closed-form solution exists via the Normal Equation |
| **Baseline** | Always the first model to try; if a non-linear model only marginally beats it, the added complexity may not be worth it |
| **Feature insight** | The magnitude and sign of learned weights reveal which features matter most |
| **Foundation** | Logistic regression, neural networks, and regularization techniques all build directly on linear regression concepts |

---

## Applications in ML

**Finance**
- Stock price forecasting
- Credit risk scoring and loan amount estimation
- Revenue and sales prediction

**Healthcare**
- Drug dosage estimation based on patient weight/age
- Predicting hospital readmission rates
- Estimating treatment costs

**Real Estate**
- House price prediction from area, location, and amenities
- Rental yield estimation

**E-commerce & Marketing**
- Customer lifetime value prediction
- Ad spend vs. conversion rate modelling
- Demand forecasting for inventory management

**Science & Engineering**
- Predicting material strength from composition
- Climate modelling (temperature trends)
- Energy consumption forecasting

---

## Projects

| Project | Description | Tech |
|---|---|---|
| [Pizza Price Prediction](linear-regression/) | Predicts pizza price from diameter using simple linear regression | Python, scikit-learn, NumPy, Jupyter |

> More projects will be added as this repository grows.

---

## Author

**Sharad Bista**

- GitHub: [@sharad-bista](https://github.com/sharad-bista)
- Email: bishalbista737@gmail.com
