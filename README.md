# Resolving Kryptonite-$n$: How Model Design Matters

This is the repository for the COMP70015 Coursework, titled _Resolving Kryptonite-$n$: How Model Design Matters.

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
- `Datasets_Train_Text_Split/`: Directory containing the dataset files (up to n=18 dimensions), split into training and testing sets. Done to ensure best hyperparameters and results of statistical tests are produced on the same split. 
- `src/`: Directory containing the source code for the project.
- `predictions/`: Directory where the predictions of the `hidden-kryptonite` datasets are saved.

Scripts:

`src/models`:
- `clustering.ipnyb`: Jupyter notebook containing the code for the cluster-based models, specifically the Gaussian Mixture Models.
- `feedforwardNN_first_implementation.ipnyb`: Jupyter notebook of our initial implementation of the neural network. It is kept because the file was used as a base for the hyper-parameter tuning of the NN, and to generate some of the graphs in our paper. For example, all of the data pre-processing graphs in the apendix were generated from this file.
- `feedforwardNN_hyper_paremeter_tuning.ipnyb`: Jupyter notebook containing the hyperparameter tuning, cross-validation, and result analysis for the neural network models.
- `k_nearest_neighbours.ipnyb`: Jupyter notebook containing the code for the k-Nearest Neighbours models, including hyperparameter optimisation, k-fold cross validation, and out-of-sample predictions.
- `polynomial_logistic_regression.ipnyb`: Jupyter notebook containing the code for the polynomial regression analysis, where the pipeline is based on the one found in the original Kryptonite paper.
- `random_forest.ipnyb`: Jupyter notebook containing the code for Random Forest, including hyperparameter optimisation, k-fold cross validation, and out-of-sample predictions.

`src/other`:
- `auc.ipnyb`: Jupyter notebook containing the code for producing AUC curves. Plots the ROC curves, and computes the AUC scores shown in the paper.
- `mcnemar_test.ipnyb`: Jupyter notebook containing the code for the McNemar test analysis. It computes the p-values for the McNemar test to compare the models we produced with the baseline logistic regression from the original Kryptonite paper.
- `train_test_split.ipnyb`: Jupyter notebook containing the code for splitting the dataset into training and testing sets.
- `vis.ipnyb`: Jupyter notebook containing the code for the visualisation of the dataset, used in Section 4.2 of the paper.