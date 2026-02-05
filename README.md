# Gold Price Forecasting Project

This project demonstrates a simple **Machine Learning + Django** based
Gold Price Forecasting system.

## 📁 Project Structure

    archive/
    │
    ├── core/                     # Django project configuration
    │   ├── setting.py
    │   ├── urls.py
    │   ├── wsgi.py
    │   └── _inti_.py
    │
    ├── gold_price/               # Django app (UI layer)
    │   └── templates/           # HTML templates (if added)
    │
    └── ml_model/                 # Machine Learning assets
        ├── gold_price_forecasting.ipynb
        ├── gold_price_forecasting_dataset.csv
        └── gold_price_linear_model.pkl

## 🎯 Objective

To predict future **gold prices** using a trained Linear Regression
model and (optionally) serve predictions via a Django web application.

## 🔧 Requirements

Install the following before running the project:

``` bash
pip install django
pip install pandas
pip install numpy
pip install scikit-learn
pip install jupyter
```

## 🚀 How to Run the ML Model

1.  Navigate to the `ml_model/` folder.
2.  Open the notebook:

``` bash
jupyter notebook gold_price_forecasting.ipynb
```

3.  Run all cells to train and save the model
    (`gold_price_linear_model.pkl`).

## 🌐 Running the Django Server (Basic)

> ⚠️ *Note: If `manage.py` is missing, create it in the root directory
> of the project.*

If present, run:

``` bash
python manage.py runserver
```

Then open in browser:

    http://127.0.0.1:8000/

## 🧠 Model Details

-   Algorithm: **Linear Regression**
-   Dataset: Historical gold price data
    (`gold_price_forecasting_dataset.csv`)
-   Output: Trained model saved as `gold_price_linear_model.pkl`

## 📌 Future Enhancements

-   Add prediction form in Django UI
-   Connect model with Django views
-   Add visualization of predictions
-   Improve model using advanced algorithms

## 👩‍💻 Author

(You can add your name here)

------------------------------------------------------------------------

If you want, I can also add steps to integrate the `.pkl` model with
Django views.
