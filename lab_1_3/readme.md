Варіант 3: Прогнозування діабету (Pima Indians Diabetes Dataset)

Опис: Прогнозування наявності діабету у пацієнтів на основі медичних характеристик.

Джерело даних: Pima Indians Diabetes Dataset

Код для завантаження:

import pandas as pd

url = "https://raw.githubusercontent.com/jbrownlee/Datasets/master/pima-indians-diabetes.data.csv"

columns = ["Pregnancies", "Glucose", "BloodPressure", "SkinThickness", "Insulin", "BMI", "DiabetesPedigreeFunction", "Age", "Outcome"]

data = pd.read_csv(url, names=columns)

X = data.iloc[:, :-1].values

y = data.iloc[:, -1].values
