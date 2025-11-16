# decision_tree_post_prunning

# Decision Tree Classifier with Post-Pruning

This repository contains an implementation of a Decision Tree Classifier with a focus on post-pruning (cost-complexity pruning) to reduce overfitting and improve generalization. The project demonstrates how pruning affects model complexity and performance.

## Overview

The notebook included in this repository covers:

* Loading and preparing a dataset
* Splitting data into features (X) and target (y)
* Training a Decision Tree Classifier before and after pruning
* Using cost-complexity pruning (`ccp_alpha`) to simplify the model
* Comparing training and testing accuracy to evaluate overfitting

## Key Concepts

### Decision Trees

A supervised learning algorithm that splits data into regions using feature-based decision rules. Each internal node represents a condition, and each leaf node represents a class prediction.

### Impurity Measures

Used to evaluate the quality of a split:

**Gini Impurity:**
[
G = 1 - \sum p_i^2
]

**Entropy:**
[
Entropy = -\sum p_i \log_2(p_i)
]

### Post-Pruning (Cost-Complexity Pruning)

A fully grown decision tree tends to overfit. Post-pruning reduces unnecessary branches by controlling model complexity using the pruning parameter `ccp_alpha`. Higher values lead to simpler trees.

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/SRDxRestricted/decision_tree_post_prunning.git
   cd decision_tree_post_prunning
   ```

2. Open the notebook:

   ```bash
   jupyter notebook decision_tree.ipynb
   ```

3. Run the cells in sequence.

## Requirements

* Python
* Jupyter Notebook
* pandas
* numpy
* scikit-learn
* matplotlib (optional)

## Future Improvements

* Compare pre-pruning and post-pruning
* Add multiple datasets
* Visualize accuracy vs. `ccp_alpha`
* Explore entropy vs. gini for different datasets

---

If you want, I can generate a version even shorter or more formal.
