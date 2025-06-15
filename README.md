# Wine Quality - Makine Öğrenmesi Projesi

Bu projede, Şaraplara ait kimyasal özellikler kullanılarak kalite puanlarını analiz etmeye ve tahmin etmeye çalıştım. Veri seti Kaggle üzerinden alındı ve temel bir veri bilimi süreci uygulandı.

## Veri Seti

Kaynak: https://www.kaggle.com/code/fedesoriano/spanish-wine-quality-dataset-introduction  
Kullanılan dosya: winequality.csv

Bu veri setinde şaraplara ait sabit asitlik, uçucu asitlik, sitrik asit, alkol oranı, sülfatlar gibi birçok özellik ve her şarap için 0–10 arasında bir kalite puanı bulunmaktadır.

## Proje Aşamaları

### 1. Veri Analizi ve Görselleştirme (EDA – Exploratory Data Analysis)

Veri setinin yapısı incelendi (satır, sütun sayısı, veri tipleri).  
Eksik değer kontrolü yapıldı.  
Bazı değişkenlerin (alkol, pH, sülfatlar) kalite ile olan ilişkisi grafiklerle gösterildi.  
Korelasyon matrisi çıkarılarak hangi değişkenlerin kaliteyle daha güçlü ilişkili olduğu görüldü.

### 2. Özellik Mühendisliği (Feature Engineering)

Şarap türü bilgisi `wine_type` adında yeni bir sütunla eklendi.  
Kalite skoru sınıflandırma için yeniden etiketlendi (örneğin: düşük, orta, yüksek kalite).  
Bazı gereksiz sütunlar çıkarıldı ya da gruplanarak sadeleştirildi.

### 3. Ön İşleme ve Dönüştürme (Preprocessing and Transformation)

Kategorik sütunlar sayısal verilere çevrildi (Label Encoding).  
Veriler ölçeklendirildi (StandardScaler ile).  
Modelleme için eğitim ve test seti oluşturuldu.

### 4. Modelleme (Model Training and Selection)

Random Forest ve Lojistik Regresyon gibi temel algoritmalar kullanıldı.  
Hem sınıflandırma (classification) hem de regresyon (regression) yöntemleri denendi.  
Model sonuçları test verisi ile değerlendirildi.

### 5. Model Değerlendirme (Model Evaluation)

Accuracy, Confusion Matrix, ve R² Score gibi metriklerle performans ölçüldü.  
Gerçek kalite puanları ile tahmin edilenler karşılaştırıldı.

## Kullanılan Araçlar

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn

## Not

Bu proje bireysel bir eğitim çalışmasıdır. Kaggle’daki örnek projeden esinlenerek yapılmıştır. Veri analizi, görselleştirme ve basit modelleme adımlarını öğrenmek amaçlıdır.