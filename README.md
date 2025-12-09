# 🏠 House Price Prediction – Machine Learning Project

Bu proje, **Kaggle – House Prices: Advanced Regression Techniques** yarışması için geliştirilmiş bir makine öğrenmesi çalışmasıdır.  
Amaç, çeşitli ev özelliklerine dayanarak **ev satış fiyatlarını tahmin eden** bir model oluşturmaktır.

---

## 📊 Kullanılan Veri

- Kaggle tarafından sağlanan **train.csv** ve **test.csv**
- Veri sayısı:
  - Train: 1.460 satır
  - Test: 1.459 satır
- Toplam 80+ özellik (kategorik + sayısal)

---

## 🧹 Veri Ön İşleme (EDA & Cleaning)

✔ Eksik değerlerin doldurulması  
✔ Kategorik değişkenlerin **One-Hot Encoding** ile dönüştürülmesi  
✔ Sayısal değişkenlerde dağılım analizi  
✔ Hedef değişken olan **SalePrice** üzerine `log` dönüşümü

---

## 🤖 Kullanılan Modeller

Aşağıdaki regresyon modelleri test edilmiştir:

| Model                                             | RMSE (Public Score) |
| ------------------------------------------------- | ------------------- |
| Linear Regression                                 | 0.1730              |
| Ridge Regression (α=50)                           | 0.1395              |
| Lasso Regression (α=0.001)                        | 0.1417              |
| Random Forest                                     | 0.1493              |
| Gradient Boosting (n_estimators=500, max_depth=3) | ⭐ **0.15073**      |

> En iyi sonuç **Gradient Boosting Regressor** modeli ile elde edilmiştir.

---

## 📦 Kullanılan Kütüphaneler

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
```

---

## 🎯 Sonuç ve Yaklaşım

- ✔ Feature engineering ve model seçimi ile skor daha da iyileştirilebilir
- ✔ XGBoost, LightGBM ve stacking yöntemleri ile geliştirmeye devam edilecektir 💡

---
