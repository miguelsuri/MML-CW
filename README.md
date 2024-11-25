# Resolving Kryptonite-$n$: How Model Design Matters

This is the repository for the COMP70015 Coursework, titled _Resolving Kryptonite-$n$: How Model Design Matters_.

The members of the group are:
- Javier Páez Franco
- Fabian Alexander Bermana
- Miguel Suriol Alfonso
- Duong Ha

## Installation

To install the required packages, run the following command:

```bash
pip install -r requirements.txt
```

## Usage

Below is an overview of the structure and the purpose of each file:

Overall structure:

- `Datasets/`: Directory containing the original dataset files used in the project.
- `Datasets_Train_Text_Split`: Directory containing the dataset files (up to $n=18$ dimensions) split into training and testing sets.
- `src/`: Directory containing the source code for the project.
- `predictions/`: Directory where the predictions of the `hidden-kryptonite` datasets are saved.

Scripts:

- `clustering.ipnyb`: Jupyter notebook containing the code for the clustering analysis, using a Gaussian Mixture Model.
- `feedforwardNN.ipnyb`: TODO
- `feedforwardNN2.ipnyb`: TODO
- `k_nearest_neighbours.ipnyb`: Jupyter notebook containing the code for the k-Nearest Neighbours analysis with hyperparameter optimisation.
- `polynomial_logistic_regression.ipnyb`: Jupyter notebook containing the code for the polynomial regression analysis, based on the original Kryptonite paper.
- `random_forest.ipnyb`: Jupyter notebook containing the code for the Random Forest analysis with hyperparameter optimisation.
- `auc.ipnyb`: Jupyter notebook containing the code for the AUC analysis. It plots the ROC curves and computes the AUC scores shown in the paper.
- `mcnemar_test.ipnyb`: Jupyter notebook containing the code for the McNemar test analysis. It computes the p-values for the McNemar test for the different models.
- `train_test_split.ipnyb`: Jupyter notebook containing the code for splitting the dataset into training and testing sets.
- `vis.ipnyb`: Jupyter notebook containing the code for the visualisation of the dataset, used in Section 4.2 of the paper.
- `vis_model_accuracies.ipnyb`: TODO