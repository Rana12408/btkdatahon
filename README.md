# btkdatahon
# 🎯 Girişimcilik Vakfı Değerlendirme Puanı Tahmini

Bu proje, Girişimcilik Vakfı'nın 2014 yılından itibaren topladığı başvuru verileri üzerinde yapılmış bir veri bilimi ve makine öğrenmesi çalışmasıdır. Projenin amacı, 2023 yılında başvuran ancak değerlendirme puanı bulunmayan 11.049 kişinin puanlarını geçmiş verileri kullanarak tahmin etmektir.

## 📊 Veri Seti Hakkında

Veri setinde, adayların aşağıdaki bilgileri yer almaktadır:

- Üniversite bilgileri  
- Aile detayları  
- İkamet bilgileri  
- Cinsiyet, yaş gibi demografik özellikler  
- 2023 yılına kadar başvuran adayların **Değerlendirme Puanı**

2023 yılında başvuran kişilerin puanları eksik olup, model bu kişilere puan tahmini yapmak üzere eğitilmiştir.

## 🔍 Proje Adımları

1. **Veri Ön İşleme:**
   - Eksik verilerin temizlenmesi
   - Kategorik değişkenlerin dönüştürülmesi
   - Anlamlı özellik mühendisliği uygulamaları

2. **Veri Görselleştirme:**
   - Değişkenler arası ilişkiler
   - Özelliklerin dağılımları

3. **Modelleme:**
   - `LightGBM`, `XGBoost`, `Random Forest` gibi algoritmalar ile regresyon modelleri oluşturuldu
   - `GridSearchCV` ile hiperparametre optimizasyonu yapıldı

4. **Değerlendirme:**
   - RMSE, MAE gibi metriklerle modeller karşılaştırıldı
   - En iyi performans gösteren model 2023 verisine uygulandı

## 📈 Kullanılan Kütüphaneler

- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
- `xgboost`
- `lightgbm`
