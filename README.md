# Student Performance Analysis

### 🎯 Layihə Haqqında

Bu layihədə şagirdlərin performansını (G3 — yekun qiymət) təhlil etmək üçün EDA (Exploratory Data Analysis), Feature Engineering, Outlier Removal, Encoding, Scaling və Linear Regression tətbiq olunmuşdur. Məqsəd — şagirdin əvvəlki göstəricilərinə əsaslanaraq yekun qiymətini proqnozlaşdırmaqdır.

### 📦 İstifadə Olunan Dataset

student-mat.csv — UCI Machine Learning Repository-dən götürülmüş real şagird məlumatları.

Atributlar: gender, yaş, təhsil səviyyəsi, ailə dəstəyi, internetə çıxış, dərs buraxmaları və s.

### 🔧 İcra olunan addımlar

**✅ 1. Məlumat Təmizliyi** 
Null və dublikat dəyərlərin yoxlanması

Uyğunsuz/outlier dəyərlərin müəyyən olunması və silinməsi (absences, failures, s.)

**✅ 2. EDA (Data Analizi)**

value_counts(), groupby() ilə statistik analizlər

Vizualizasiya: histplot, boxplot, scatterplot, pie chart, countplot, heatmap

**✅ 3. Encoding & Scaling** 

LabelEncoding (binary sütunlar)

One-Hot Encoding (Mjob, Fjob, guardian, school, reason)

StandardScaler (G1, G2, G3)

MinMaxScaler (age, absences)

**✅ 4. Model Quruluşu** 

Model: LinearRegression

Qiymətləndirmə metrikləri:

MAE ≈ 1.44

RMSE ≈ 2.03

R² ≈ 0.85

### 📊 Ən Təsirli Xüsusiyyətlər

Xüsusiyyət	Təsir
G2	✅ Güclü pozitiv təsir
G1	✅ Müsbət təsir
failures	❌ Güclü mənfi təsir
higher	✅ Müsbət niyyət
Medu	✅ Zəif, amma pozitiv

### 📌 Nəticə
Model G3 qiymətini yüksək dəqiqliklə təxmin edə bilir. Əvvəlki qiymətlər (G1, G2) və təhsil motivasiyası (ali təhsil istəyi, valideyn təhsili) ən vacib amillərdir.

### 🧪 İstifadə Olunan Kitabxanalar
python
Copy
Edit
pandas, numpy, seaborn, matplotlib, scikit-learn

### 🚀 Necə İstifadə Etməli:
student-mat.csv faylını content/ qovluğuna əlavə et.

student_performance.py və ya .ipynb faylını çalıştır.

Qrafiklər, təhlillər və proqnozlar terminal və ya notebook üzərindən görünəcək.

