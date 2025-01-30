**Breast Cancer Classification**
Dataset yang digunakan adalah Load_breast_cancer dari sklearn. Dataset ini berisi informasi mengenai kanker payudara yang digunakan secara luas untuk keperluan pembelajaran dan eksperimen dalam bidang machine learnig, khususnya dalam klasifikasi. Dataset ini berfokus pada diagnosis kanker payudara dengan fitur-fitur pada massa tumor seperti ukuran dan bentuk. Dataset ini berisi dua kategori kelas yaitu malignant (kanker ganas) dan benign (kanker jinak).
Dataset ini terdiri dari 569 sampel dan 30 fitur yang diukur dari citra dgital payudara. Beberapa fitur yang ada dalam dataset adalah: 
1. Radius (mean, standar eror, dan largest)
2. Texture (mean, standar eror, dan largest)
3. Perimeter (mean, standar eror dan largest)
4. Area (mean, standar eror dan largest)
5. Smoothness, compactness, concavity, dll

**Cara Menggunakan**
Untuk memuat dataset ini anda dapat menggunakan fungsi Load_breast_cancer dari pustaka sklearn.datasets:

from sklearn.datasets import load_breast_cancer
import pandas as pd

# Load dataset
data = load_breast_cancer()

# Convert to Pandas DataFrame
df = pd.DataFrame(data.data, columns=data.feature_names)
df['Target'] = data.target

# Display first 5 rows
print(df.head())

**Tahapan-Tahapan**
1. EDA (Exploratory Data Analysis)
2. Building a Machine Learning Model
3. Visualisasi
