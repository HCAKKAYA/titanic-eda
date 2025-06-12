# 🚢 Titanic: Hayatta Kalma Tahmini (Machine Learning Projesi)

Bu proje, Titanic yolcularının hayatta kalıp kalmadığını tahmin etmeye yönelik bir makine öğrenmesi uygulamasıdır. Veri, [Kaggle Titanic Competition](https://www.kaggle.com/competitions/titanic) sayfasından alınmıştır ve başlangıç seviyesindeki veri bilimi projelerine örnek teşkil eder.

## 🔍 Problem Tanımı

Titanic kazasında hayatta kalma ihtimali, kişinin özelliklerine göre (yaş, cinsiyet, bilet sınıfı vb.) değişkenlik göstermiştir. Bu projede amaç, yolcuların verilerine bakarak bir kişinin hayatta kalıp kalmadığını tahmin eden bir model geliştirmektir.

## 📦 Kullanılan Veri Setleri

- `train.csv`: Modelin eğitildiği etiketli veri (Survived bilgisi var)
- `test.csv`: Tahmin yapılacak etiketlenmemiş veri (Survived bilgisi yok)
- `gender_submission.csv`: Kaggle’ın örnek gönderim dosyası (şablon)

## 🛠 Kullanılan Kütüphaneler

- pandas
- numpy
- matplotlib / seaborn (EDA için)
- scikit-learn

## 🧪 Yapılan Aşamalar

### 1. Veri Analizi (EDA)

- Eksik verilerin tespiti ve analizi
- Cinsiyet, yaş, sınıf gibi değişkenlerin hayatta kalmaya etkisi
- Görselleştirme ile öngörü çıkarımı

### 2. Veri Ön İşleme

- Eksik değerlerin doldurulması
- Kategorik verilerin sayısallaştırılması
- Yeni değişken üretimi (`FamilySize`, `IsAlone`)
- Gereksiz sütunların çıkarılması (`Name`, `Ticket`, `Cabin`)

### 3. Modelleme

- `Logistic Regression` modeli ile ilk tahminler
- Model doğruluk skorlarının ölçülmesi (`accuracy`, `classification_report`)
- `test.csv` üzerinde tahmin yapılması

### 4. Sonuçların Kaydedilmesi

- Tahminler `submission.csv` dosyasına kaydedildi
- Dosya formatı Kaggle yarışması ile uyumlu

## 📊 Örnek Tahmin Formatı

- PassengerId,Survived
- 892,0
- 893,1
- 894,0

## ✅ Sonraki Geliştirme Fikirleri

- Random Forest, XGBoost gibi daha güçlü modellerle karşılaştırma
- `Title`, `FareBand`, `AgeBand` gibi yeni özellik mühendisliği denemeleri
- GridSearchCV ile hiperparametre optimizasyonu
- Kaggle’da puan artırmaya yönelik denemeler

## 📁 Proje Yapısı

- titanic_project/
- train.csv
- test.csv
- gender_submission.csv
- submission.csv
- titanic_model.ipynb
- README.md

## 👤 Yazar

- Hüseyin Akkaya
