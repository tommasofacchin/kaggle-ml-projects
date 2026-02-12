Kaggle ML Projects
==================

This repository collects my **machine learning projects based on Kaggle notebooks**, with a focus on **computational intelligence and deep learning** applied to practical problems.
Each project has its own notebook and sometimes an additional report on the `report` folder.

The goal of this repo is to build a small, coherent portfolio of end‑to‑end ML experiments, rather than isolated scripts or competition submissions, and to use each project as a way to systematically learn and try out new ideas in computational intelligence and deep learning.

---

## Projects

### 1. Genetic Algorithm from Scratch

This project implements a generic **genetic algorithm (GA) from scratch in Python** and walks through several practical examples, from toy optimization problems to a small ML use case. 
The core of the project is a reusable `GeneticAlgorithm` class that encapsulates the full GA loop (initialization, selection, crossover, mutation, elitism, history tracking), while letting you plug in your own representation, fitness function, and genetic operators.

The notebook includes:
- A clean implementation of the `GeneticAlgorithm` class with configurable operators and hyperparameters.
- Examples on bitstring optimization (OneMax) and other simple tasks.
- A feature‑selection example where the GA evolves binary masks for a real ML model (logistic regression).
- Plots of convergence and basic diagnostics to understand how the GA behaves across generations.

> 🔗 Kaggle notebook: [here](https://www.kaggle.com/code/tommasofacchin/genetic-algorithm-from-scratch)
> 
> 🔗 Github repo: [here](https://github.com/tommasofacchin/genetic-algorithm-from-scratch)

---

### 2. Symbolic Regression for Building Heating Load

This project uses the Energy Efficiency dataset (residential buildings) to predict **heating load** from 8 design and geometric features such as surface area, wall area, roof area, glazing area, and overall height.

I train a high‑accuracy Random Forest model and then apply **symbolic regression (PySR)** to discover explicit formulas that approximate the same target.  
The main idea is to compare a very accurate black‑box model with simpler, human‑readable equations, and to study the trade‑off between **accuracy** and **interpretability**.

The notebook includes:
- Data loading and basic preprocessing.
- Random Forest training and evaluation (RMSE, MAE, R²).
- PySR setup and search over symbolic expressions.
- Selection of a final symbolic model and comparison with the Random Forest, both via metrics and a few concrete prediction examples.


> 🔗 Kaggle notebook: [here](https://www.kaggle.com/code/tommasofacchin/symbolic-regression-energy-efficiency)
