# HealthCare-ML
Machine Learning project for Global AI Hub

# 🏥 Healthcare Billing Amount Prediction

Bu proje, gözetimli öğrenme algoritmalarını kullanarak hastaların verilerine göre **hastane fatura tutarını (billing amount)** tahmin etmeyi amaçlamaktadır.

---

## 📊 Kullanılan Algoritmalar ve Nedenleri

Bu projede aşağıdaki iki algoritma test edilmiştir:

1. **Linear Regression**  
   Basit ve yorumlanabilir bir regresyon algoritmasıdır. Doğrusal ilişkileri iyi modeller.

2. **Decision Tree Regressor** ✅  
   Karar ağaçları, değişkenler arasındaki karmaşık ilişkileri öğrenebilir ve aşırı veri ön işleme ihtiyacı duymaz.  
   Yapılan çapraz doğrulama sonucunda daha düşük hata verdiği için bu model seçilmiştir.

> Seçilen model: **Decision Tree Regressor (GridSearchCV ile optimize edilmiştir)**

---

## 📁 Veri Seti Açıklaması

Veri seti, her hasta için şu bilgileri içermektedir:

- Demografik bilgiler (yaş, cinsiyet, kan grubu)
- Tıbbi durumlar (hastalık, ilaç, test sonuçları)
- Yatış bilgileri (giriş-çıkış tarihi, yatış türü)
- Faturalama bilgileri (sigorta, hastane, doktor, oda no)
- Etiket (target): **`billing_amount`** (gerçek sayısal değer)

Bu veri seti, [Kaggle - Healthcare Dataset](https://www.kaggle.com/datasets/prasad22/healthcare-dataset) üzerinden alınmıştır ve 10.000’den fazla satır içermektedir.

---

## 🌍 Problemin Gerçek Hayattaki Karşılığı

Hastaneler ve sigorta şirketleri için:
- Fatura tahmini yaparak önceden maliyet planlaması,
- Hasta başvurusunda tahmini maliyet bilgilendirmesi,
- Anormal faturalamaları tespit etme

...gibi birçok iş sürecine katkı sağlayabilir.

---

## 📈 Sonuçların Yorumlanması

**Optimize Edilmiş Model Performansı (Decision Tree):**

- MAE (Ortalama Mutlak Hata): ~3184 TL  
- RMSE (Kök Ortalama Kare Hata): ~4161 TL  
- R² Skoru: 0.87

Model, fatura tutarlarını oldukça isabetli tahmin edebilmekte ve verilerin %87’sini açıklayabilmektedir.

---

## 🔗 Kaggle Linki

> Projenin Kaggle notebook bağlantısı:  
> 📎 [https://www.kaggle.com/yaskucuker/healthcare-billing-prediction](https://www.kaggle.com/work/collections/15975042)
> 📎 [https://www.kaggle.com/yaskucuker/healthcare-billing-prediction](https://www.kaggle.com/code/yaskucuker/algorithm2)
> 📎 [https://www.kaggle.com/yaskucuker/healthcare-billing-prediction](https://www.kaggle.com/code/yaskucuker/datavisualization)

