# Aygaz-Yapay-Zekaya-Giris-Bootcamp
# Proje Özeti
Bu proje, görüntülerden oluşan bir veri setini çeşitli makine öğrenmesi ve derin öğrenme teknikleri ile daha okunabilir ve gözlemlenebilir hale getirmeyi amaçlamaktadır. Çalışma sürecinde farklı modellerin performansları karşılaştırılmış ve en iyi sonuçlar belirlenmiştir.

## İçindekiler
1. [Kullanılan Kütüphaneler](#kullanılan-kütüphaneler)
2. [Veri Hazırlama](#veri-hazırlama)
3. [Makine Öğrenmesi Modelleri](#makine-öğrenmesi-modelleri)
4. [Derin Öğrenme Modelleri](#derin-öğrenme-modelleri)
5. [Sonuçlar](#sonuçlar)
6. [Referanslar ve Kaynaklar](#referanslar-ve-kaynaklar)

---

## Kullanılan Kütüphaneler
Bu projede aşağıdaki Python kütüphaneleri kullanılmıştır:
- `pandas`: Veri manipülasyonu ve analizi.
- `numpy`: Matematiksel hesaplamalar.
- `matplotlib`: Veri görselleştirme.
- `seaborn`: Veri analizi ve istatistiksel görselleştirme.
- `scikit-learn`: Makine öğrenmesi modelleri ve metrikleri.

---

## Veri Hazırlama
Proje için kullanılan veri seti, **fashion_mnist** olarak adlandırılmıştır. Bu veri seti, giyim ürünlerini (ayakkabı, gömlek, çanta vb.) içermektedir. Veri seti aşağıdaki gibi işlenmiştir:

1. **Eğitim ve Test Kümelerine Ayırma**:
   - Eğitim kümeleri, modellerin eğitilmesi için kullanılmıştır.
   - Test kümeleri, modellerin performansını değerlendirmek için kullanılmıştır.

2. **Normalizasyon ve Dönüştürmeler**:
   - Piksel değerleri [0,1] arasına çekilmiştir.
   - Veriler numpy dizilerine dönüştürülmüştür.

3. **Etiketlerin Kodlanması**:
   - Veri setindeki kategorik etiketler, modellerin işlemesi için birer numerik değere dönüştürülmüştür.

---

## Makine Öğrenmesi Modelleri
Projede aşağıdaki makine öğrenmesi algoritmaları kullanılmıştır:

### Kullanılan Algoritmalar
1. **K-Nearest Neighbors (KNN)**:
   - Veriye en yakın komşuları temel alarak sınıflandırma yapar.
   - Performansı hız ve doğruluk açısından tatmin edicidir.

2. **Support Vector Classifier (SVC)**:
   - Veriyi daha iyi ayırabilmek için hiperdüzlemler kullanır.
   - Yüksek doğruluk oranına sahip ancak yavaş bir işlem süresi vardır.

3. **Random Forest**:
   - Birden fazla karar ağacından oluşan bir ensemble modeldir.
   - Dengeli bir performans sunar.

4. **Decision Tree**:
   - Veri setini dallara ayırarak sonuca ulaşır.
   - Hızlı ancak genellikle düşük doğruluk oranı sunar.

### Performans Metrikleri
- **Accuracy**: Doğru tahmin edilen sınıfların toplam tahminlere oranı.
- **Precision**: Pozitif olarak tahmin edilenlerin kaçının gerçekte pozitif olduğu.
- **Recall**: Gerçekte pozitif olanların kaçının doğru tahmin edildiği.
- **F1 Score**: Precision ve Recall'un harmonik ortalaması.

### Performans Değerlendirmesi
- **SVC**: En iyi performansı göstermiştir ancak en uzun işlem sürecine sahiptir.
- **KNN**: En hızlı çalışmış ve iyi performans sergilemiştir.
- **Decision Tree**: En kötü performansı göstermiştir.

---

## Derin Öğrenme Modelleri
Projede iki temel derin öğrenme modeli kullanılmıştır:

### Kullanılan Modeller
1. **Yapay Sinir Ağları (YSA)**:
   - Tam bağlantılı katmanlardan oluşan klasik bir sinir ağı yapısı.
   - "adadelta" optimizasyon parametresi ile en iyi performans elde edilmiştir.

2. **Convolutional Neural Networks (CNN)**:
   - Görüntü işleme için özel olarak tasarlanmış katmanlar içerir.
   - "adam" optimizasyon parametresi ile daha iyi sonuçlar elde edilmiştir.

### Performans Değerlendirmesi
- **YSA**: Veri setinde "adadelta" optimizasyon algoritmasını kullanarak etkili bir performans sergilemiştir.
- **CNN**: Daha karmaşık yapısı sayesinde en iyi sonuçları sağlamıştır.

---

## Sonuçlar
- **Makine Öğrenmesi Modelleri**:
  - En iyi performansı **SVC** modeli göstermiştir.
  - KNN, hızlı bir alternatif olarak tatmin edici bir performans sergilemiştir.
  - Decision Tree modeli, beklenenin altında performans göstermiştir.

- **Derin Öğrenme Modelleri**:
  - **CNN**, "adam" optimizasyonu ile en iyi performansa ulaşmıştır.
  - **YSA**, daha basit bir model olarak "adadelta" ile etkili bir performans sergilemiştir.

---

## Referanslar ve Kaynaklar
1. [Fashion MNIST Dataset](https://github.com/zalandoresearch/fashion-mnist)
2. [Scikit-Learn Documentation](https://scikit-learn.org/stable/documentation.html)
3. [Keras Documentation](https://keras.io/)
4. [Numpy Documentation](https://numpy.org/doc/)
5. [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)


