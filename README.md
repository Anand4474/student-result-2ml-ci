# Student Result Prediction ML CI

Student Result Prediction machine-learning model with GitHub Actions CI and an accuracy quality gate.

## Features
- Reproducible dataset generation
- Logistic Regression classifier
- Accuracy and confusion matrix
- Saved model and metrics
- ML quality gate (minimum accuracy 0.85)
- Automated ML tests
- GitHub Actions CI

## Input Features
- attendance
- internal_marks
- assignment_marks
- previous_score

## Target
- 1 = PASS
- 0 = FAIL

## Local Commands (VS Code terminal)
```
python -m venv .venv
.venv\Scripts\activate          # Windows
pip install -r requirements.txt
python train_model.py
python quality_gate.py
python -m unittest discover -v
```
