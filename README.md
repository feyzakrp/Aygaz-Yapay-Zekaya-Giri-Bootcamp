# Aygaz-Yapay-Zekaya-Giri-Bootcamp

## Proje Özeti
Bu proje, görüntülerden oluşan bir veri setini çeşitli makine öğrenmesi ve derin öğrenme teknikleri ile daha okunabilir ve gözlemlenebilir hale getirmeyi amaçlamaktadır.

## İçindekiler
- [Kullanılan Kütüphaneler]
- [Veri Hazırlama]
- [Makine Öğrenmesi Modelleri]
- [Derin Öğrenme Modelleri]
- [Sonuçlar]
- [Referanslar ve Kaynaklar]

Kullanılan Kütüphaneler
pandas
numpy
matplotlib
seaborn
scikit-learn

 Veri Hazırlama
Veri seti fashion_mnist olarak adlandırılmıştır ve ayakkabı, gömlek, çanta gibi giyim ürünlerini içermektedir. Bu veri seti eğitim ve test kümelerine ayrılmıştır.

Makine Öğrenmesi Modelleri
Kullanılan algoritmalar:

K-Nearest Neighbors (KNN)
Support Vector Classifier (SVC)
Random Forest
Decision Tree
Performans metrikleri olarak accuracy, recall, f1 score ve precision değerleri kullanılmıştır.

Performans Değerlendirmesi
SVC: En iyi performansı gösteren modeldir, ancak en uzun işlem süresine sahiptir.
KNN: En kısa sürede iyi performans sergilemiştir.
Decision Tree: En kötü performansı göstermiştir.
Derin Öğrenme Modelleri
Kullanılan modeller:

Yapay Sinir Ağları (YSA)
Convolutional Neural Networks (CNN)
Performans Değerlendirmesi
YSA: "adadelta" parametresi ile en iyi performansı göstermiştir.
CNN: "adam" parametresi ile daha iyi sonuçlar elde edilmiştir.
Sonuçlar
Makine öğrenmesi modellerinden en iyi performansı SVC göstermiştir.
Derin öğrenme modellerinden en iyi performansı YSA (adadelta parametresi ile) göstermiştir.
