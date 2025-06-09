# Titanic - Makine Öğrenmesi Projesi

Bu proje, Titanic faciası sırasında yolcuların hayatta kalıp kalamayacağını tahmin etmek için makine öğrenmesi teknikleri kullanılarak hazırlanmıştır.

## Veri Seti

Kaynak: https://www.kaggle.com/competitions/titanic  
Kullanılan dosyalar: train.csv, test.csv

## Proje Aşamaları

1. Veri Analizi ve Görselleştirme (EDA - Exploratory Data Analysis)  
   Eksik değerler, aykırı değerler ve dağılımlar incelendi.  
   Cinsiyet, yaş, sınıf gibi değişkenlerin hayatta kalma üzerindeki etkisi analiz edildi.

2. Özellik Mühendisliği (Feature Engineering)  
   Yeni değişkenler türetildi. Örneğin: FamilySize, IsAlone, Title gibi sütunlar oluşturuldu.  
   Mevcut verilerden daha anlamlı yapılar üretildi.

3. Ön İşleme ve Dönüştürme (Preprocessing and Transformation)  
   Eksik veriler dolduruldu.  
   Kategorik veriler sayısal hale getirildi (One-Hot Encoding, Label Encoding).  
   Sayısal veriler uygun şekilde ölçeklendirildi.

4. Modelleme (Model Training and Selection)  
   Logistic Regression, Random Forest, XGBoost gibi algoritmalar denendi.  
   Eğitim ve test ayrımı yapılara performans ölçüldü.

5. Model Değerlendirme (Model Evaluation)  
   Accuracy, ROC AUC ve Confusion Matrix gibi metriklerle değerlendirme yapıldı.  
   Modellerin başarıları karşılaştırıldı.

## Kullanılan Kütüphaneler

pandas  
numpy  
matplotlib  
seaborn  
scikit-learn

## Proje Yapısı

01_Titanic/  
├── data/  
│   ├── train.csv  
│  
├── notebook/  
│   └── titanic.ipynb  
├── images/  
│   └── grafik dosyaları (varsa)  
├── README.md  
├── requirements.txt  
└── .gitignore

## Notlar

Bu proje, veri analizinden modellemeye kadar uçtan uca bir veri bilimi sürecini kapsamaktadır. Özellik mühendisliği, model karşılaştırması ve veri sızıntısı kontrolü gibi temel veri bilimi prensiplerine uygun şekilde ilerlenmiştir. Eğitim ve test verileri ayrı tutulmuş, sonuçlar objektif şekilde değerlendirilmiştir.