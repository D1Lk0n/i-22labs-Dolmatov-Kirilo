Варіант 3: Wine Quality Dataset
Опис: Прогнозування якості вина на основі його фізико-хімічних властивостей.
Джерело даних: UCI Wine Quality Dataset
Отримання та використання даних:
1.	Завантажте файл даних з https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv
2.	Дані представлені у форматі CSV з розділювачем ";"
3.	Використовуйте pandas для завантаження даних:
import pandas as pd
url = "https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv"
df = pd.read_csv(url, sep=';')
# Виберіть features (X) та цільову змінну (y)
X = df.drop('quality', axis=1).values
y = df['quality'].values
Рекомендовані параметри для початку:
•	w_init = np.zeros(X.shape[1])
•	b_init = 0
•	alpha = 0.0001
•	iterations = 2000
