# 🦋 Butterfly Image Classification (CNN)

## 📑 İçindekiler
- [Proje Özeti](#proje-özeti)
- [Veri Seti](#veri-seti)
- [Projenin Amacı](#projenin-amacı)
- [Model Yapısı](#model-yapısı)
- [Hiperparametre Optimizasyonu](#hiperparametre-optimizasyonu)
- [Kaggle Proje Linki](#kaggle-proje-linki)

---

## Proje Özeti
Bu projede, farklı kelebek türlerini sınıflandırmak için **Convolutional Neural Network (CNN)** kullanılmıştır. Veri seti, Kaggle’da bulunan “Butterfly Image Classification” veri seti kullanılarak hazırlanmıştır. Model, görüntülerden öğrenerek 75 farklı kelebek sınıfını tanımayı hedeflemektedir.  

---

## 🛢️ Veri Seti
Veri seti aşağıdaki özellikleri taşımaktadır:  
- Toplam sınıf sayısı: 75  
- Toplam görüntü sayısı: 6499
- Görüntü formatı: 224x224 RGB

Veri seti **train/validation/test** olarak ayrılmış ve modelin genelleme kabiliyeti test edilmiştir.

---

## 🎯 Projenin Amacı
Bu projenin temel amacı, CNN kullanarak kelebek türlerini doğru şekilde sınıflandırmak ve modelin genelleme kabiliyetini artırmaktır.  
- Aşırı öğrenmeyi önlemek için **Dropout** ve **Batch Normalization** kullanılmıştır.  
- Hiperparametre ayarları ile modelin doğruluk performansı optimize edilmeye çalışılmıştır.  

---

## 🧠 Model Yapısı
Modelin genel yapısı şu şekildedir:  
1. **Girdi Katmanı:** Görüntü pikselleri doğrudan CNN’e beslenir.  
2. **Convolutional Katmanlar:** Özellik çıkarımı yapılır.  
3. **Batch Normalization ve Dropout:** Aşırı öğrenmeyi engeller ve modelin stabilitesini artırır.  
4. **Flatten ve Dense Katmanlar:** Sınıflandırma yapılır.  
5. **Çıktı Katmanı:** 75 sınıf için **softmax** aktivasyon fonksiyonu kullanılır.  

---

## 🚀 Hiperparametre Optimizasyonu
- Modelin performansını artırmak amacıyla farklı optimizasyon teknikleri (**Adam, RMSprop, SGD**) denendi.  
- Learning rate ve batch size gibi parametreler test edildi.  
- En iyi doğruluk %79.9 olarak elde edilmiştir.  

---

-Model test veri seti üzerinde güçlü bir performans göstermiştir ve genel olarak iyi genelleme kabiliyeti sunmaktadır.  
- Transfer learning yöntemleri ile performans artırılabilir.  
- Hiperparametre optimizasyonu için Bayesian Optimization gibi yöntemler denenebilir.  

---

## 🔗 Kaggle Proje Linki
Projenin Kaggle sayfasına ulaşmak için: [Butterfly Classification (CNN)] https://www.kaggle.com/code/gulcinyzglc/butterfly-image-classification-with-cnn


