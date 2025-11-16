# Decision_tree

# Decision Tree Classifier with Pre-Pruning and Post-Pruning

This repository contains an implementation of a Decision Tree Classifier demonstrating both **pre-pruning** and **post-pruning** techniques to control model complexity and reduce overfitting. The project shows how different pruning strategies affect decision tree depth, structure, and accuracy on training and testing data.

## Overview

The notebook covers:

* Loading and preparing the dataset
* Splitting data into features (X) and target (y)
* Training a Decision Tree without pruning (full tree)
* Applying **pre-pruning** using hyperparameters such as:

  * `max_depth`
  * `min_samples_split`
  * `min_samples_leaf`
  * `max_leaf_nodes`

* Comparing performance before and after pruning

## Key Concepts

### Decision Tree

A supervised classification algorithm that recursively splits data based on feature conditions. Each internal node represents a decision rule; each leaf node represents a class prediction.

### Impurity Measures

Used for evaluating the quality of splits:

**Gini Impurity**
[
G = 1 - \sum p_i^2
]

**Entropy**
[
Entropy = -\sum p_i \log_2(p_i)
]

### Pre-Pruning

Pre-pruning restricts tree growth by limiting depth or requiring a minimum number of samples to split. This prevents overly complex trees and reduces overfitting early during training.

### Post-Pruning 

Post-pruning first grows a full tree, then prunes branches that provide minimal improvement.


## Running the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/SRDxRestricted/Decision_tree.git
   cd Decision_tree
   ```
2. Open the notebook:

   ```bash
   jupyter notebook decision_tree.ipynb
   ```
3. Execute the notebook cells sequentially.

## Requirements

* Python
* Jupyter Notebook
* pandas
* numpy
* scikit-learn
* matplotlib (optional)

## Future Improvements

* Visual comparison of tree structures before and after pruning
* Experiments with different datasets
* Grid search for optimal `ccp_alpha` and pre-pruning parameters
* Entropy vs Gini performance comparison

---

If you want, I can also create a **minimal version**, a **highly detailed version**, or even a **README with images/plots** once you upload screenshots.
