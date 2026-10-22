# HealthBloom

A Flask web app that predicts the risk of common diseases from health parameters. Users create an account, sign in and use the disease predictors from a personal dashboard.

## Features

- **Heart disease prediction** (`heart.pkl`)
- **Diabetes prediction** (`d.pkl`)
- **Blood pressure abnormality prediction** (`bp.pkl`)
- **User accounts:** sign-up and login with Flask-Login, Flask-WTF forms and an SQLite database

All three models are Random Forest classifiers trained with scikit-learn. The training scripts are in `models/`, and the datasets are in `dataset/`.

## Tech stack

Python, Flask, Flask-SQLAlchemy, Flask-Login, Flask-Bootstrap, scikit-learn, pandas, gunicorn

## Getting started

```bash
pip install -r requirements.txt
python app.py
```

Then open http://127.0.0.1:5000. A `Procfile` is included for Heroku deployment.

> For learning purposes only. This is not a substitute for medical advice.
