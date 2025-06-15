# 🎓 Student Addiction Analysis - ML Classification Project

Bu proje, öğrenciler arasında bağımlılık riski taşıyan bireylerin belirlenmesi amacıyla gerçekleştirilmiştir. Veri bilimi ve makine öğrenimi teknikleri kullanılarak, risk faktörlerinin analizi yapılmış ve tahmin modelleri geliştirilmiştir.

## 📁 Proje İçeriği

- `student_addiction_dataset_train.csv`  
- `student_addiction_dataset_test.csv`  
- `student_addiction_analysis.ipynb`  
- `StudentAddictionAnalysis.docx` (proje raporu)  
- `README.md` (bu dosya)

## 🎯 Proje Amacı

Bu çalışmanın temel hedefi, çeşitli davranışsal ve psikososyal faktörler doğrultusunda bir öğrencinin bağımlılık riskini tahmin edebilen bir sınıflandırma modeli geliştirmektir. Bu modelin eğitim kurumlarında erken müdahale ve destek süreçlerinde kullanılabilir olması amaçlanmaktadır.

## 🧠 Kullanılan Özellikler (Feature Set)

| Özellik | Açıklama |
|--------|----------|
| `Experimentation` | Yeni madde deneme geçmişi |
| `Academic_Performance_Decline` | Akademik başarıda düşüş |
| `Social_Isolation` | Sosyal çevreden kopma durumu |
| `Financial_Issues` | Maddi zorluklar yaşanması |
| `Physical_Mental_Health_Problems` | Sağlık problemleri |
| `Legal_Consequences` | Yasal sorunlar yaşama |
| `Relationship_Strain` | Aile/arkadaş ilişkilerinde gerilim |
| `Risk_Taking_Behavior` | Riskli davranışlar sergileme |
| `Withdrawal_Symptoms` | Yoksunluk belirtileri gözlemlenmesi |
| `Denial_and_Resistance_to_Treatment` | Tedaviye karşı direnç gösterme |
| `Addiction_Class` | Hedef değişken (Bağımlı / Bağımlı Değil) |

## ⚙️ Kullanılan Yöntemler

- Label Encoding & Eksik Veri Temizleme
- Feature Importance Analizi
- Gradient Boosting Classifier
- ROC Curve, Confusion Matrix, AUC Score
- SMOTE (dengesiz veri çözümü önerisi)

## 📊 Model Performansı (Gradient Boosting)

| Metrik | Değer |
|--------|-------|
| Doğruluk (Accuracy) | %85 |
| ROC-AUC | 0.68 |
| F1-score (Bağımlı sınıf) | 0.51 |

> **Not:** AUC skorunun görece düşük olması, sınıflar arası dengesizliğe işaret etmektedir. SMOTE ve daha dengeli veri ile bu durum iyileştirilebilir.

## 🔍 Öne Çıkan Bulgular

- `Denial_and_Resistance_to_Treatment` ve `Academic_Performance_Decline`, bağımlılık sınıfını en iyi ayıran değişkenlerdir.
- Model, bağımlı olmayan sınıfı daha iyi tanırken, bağımlı sınıfı tespit etmede zorlanmaktadır.
- Veri dengesizliği, performansı olumsuz yönde etkilemektedir.

## 💡 Gelecek Geliştirmeler

- SMOTE uygulaması ile veri dengesi sağlanacak.
- XGBoost, LightGBM gibi gelişmiş modellerle karşılaştırmalı analiz yapılacak.
- Demografik veri (yaş, cinsiyet, eğitim türü vb.) eklenerek modelin zenginleştirilmesi planlanmaktadır.
- Power BI veya Dash ile etkileşimli dashboard hazırlanabilir.

## 📚 Gereksinimler

```bash
Python 3.8+
pandas
numpy
matplotlib
seaborn
scikit-learn
