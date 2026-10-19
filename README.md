# Iris Flower Classification Using Machine Learning

## Project overview
This beginner machine learning project predicts an Iris flower's species from four measurements: sepal length, sepal width, petal length, and petal width. It trains and compares two supervised classification models: a Decision Tree and K-Nearest Neighbors (KNN).

## Dataset
The project uses the Iris dataset bundled with scikit-learn. It contains 150 samples, four numerical features, and three species classes.

- Dataset documentation: https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_iris.html
- Original UCI dataset page: https://archive.ics.uci.edu/dataset/53/iris

The notebook loads the dataset directly through scikit-learn, so a separate CSV download is not required.

## Files
- `Iris_Flower_Classification.ipynb` — complete notebook with data preparation, model training, evaluation, confusion matrices, and conclusion.
- `README.md` — project overview and setup instructions.

## Setup and run
### Recommended: Google Colab
1. Open https://colab.research.google.com/
2. Select **File → Upload notebook** and upload `Iris_Flower_Classification.ipynb`.
3. Select **Runtime → Run all**.
4. Review the accuracy table, confusion matrices, and generated conclusion.

### Run locally with Jupyter
Install Python 3, then run:

```bash
python -m pip install pandas matplotlib seaborn scikit-learn notebook
jupyter notebook
```

Open `Iris_Flower_Classification.ipynb` and run all cells in order.

## Data preparation
- Inspected the dataset and its shape.
- Checked missing values and duplicate rows.
- Used four measurement columns as features and species as the target.
- Split data into 80% training and 20% testing sets using a fixed random seed and stratified sampling.
- Standardized features for KNN inside a pipeline.

## Models and evaluation
The notebook compares:
1. Decision Tree Classifier
2. K-Nearest Neighbors (KNN), with `k=5`

Evaluation includes test accuracy, confusion matrices, and classification reports (precision, recall, and F1-score).

**Results (fixed test split with `random_state=42`):** Decision Tree accuracy = **93.33%**; KNN accuracy = **93.33%**. Both models achieved the same accuracy on this split. Your results should match when you run the notebook with the same scikit-learn dataset and settings.

## Conclusion
The notebook prints which model has higher accuracy on the selected test split. The better result is specific to this split and does not guarantee that the same model will perform best on every dataset. This project demonstrates the basic machine learning workflow: data inspection, preparation, model training, and evaluation.

## Author
Add your name here before submitting.
