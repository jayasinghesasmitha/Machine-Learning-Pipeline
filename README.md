## Machine Learning Pipeline with Scikit-Learn

### Description
This repository contains a Machine Learning pipeline built using Python and Scikit-Learn. The pipeline includes data preprocessing, model training, and evaluation.

### Features
- Data preprocessing with `SimpleImputer`
- Model training using `LogisticRegression`
- Pipeline creation using `make_pipeline`
- Hyperparameter tuning and evaluation

### Installation
Ensure you have Python installed, then install the required libraries:

```sh
pip install scikit-learn pandas numpy jupyter
```

### Usage
Run the Jupyter Notebook to see the pipeline in action:

```sh
jupyter notebook pipeline.ipynb
```

### Example Code
```python
from sklearn.pipeline import make_pipeline
from sklearn.impute import SimpleImputer
from sklearn.linear_model import LogisticRegression

# Define components
imputer = SimpleImputer(strategy="mean")
lr = LogisticRegression()

# Create pipeline
pipe = make_pipeline(imputer, lr)
print(pipe)
```
