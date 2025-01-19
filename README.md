### Proje: Makine Öğrenmesi ile Sürdürülebilir Görsel İletişim Verisi Analizi

---

#### Giriş

Bu proje, sürdürülebilir tasarım verisi üzerinde eksik veri yönetimi ve veri analizi yapmayı amaçlayan kapsamlı bir Python uygulamasıdır. Projede, eksik verilerin farklı yöntemlerle doldurulması ve ardından bu yöntemlerin performanslarının karşılaştırılması hedeflenmiştir. Kod, aynı zamanda makine öğrenmesi modelleriyle verilerin değerlendirilmesi ve anlamlı çıkarımlar yapılmasını sağlar.

Veriseti : https://www.kaggle.com/datasets/ziya07/visual-communication-art-design-data

---

#### Proje Yapısı ve Amaçları

1. **Eksik Verilerin Doldurulması**  
   Hem sayısal hem de kategorik değişkenlerde eksik veri sorunlarını gidermek için çeşitli yöntemler kullanılmıştır:
   - Sayısal eksik veriler: Ortalama, medyan, KNN Imputer, tahmin modelleri gibi yöntemler.
   - Kategorik eksik veriler: Mod ile doldurma, "Bilinmiyor" etiketi, tahmine dayalı doldurma.

2. **Veri Setinin Zenginleştirilmesi**  
   Her eksik değer doldurma yöntemi için ayrı veri setleri oluşturulmuş ve bunlar daha sonra analiz edilmek üzere bir diziye kaydedilmiştir.

3. **Performans Karşılaştırması**  
   Eksik veri doldurma yöntemlerinin, veri analizi ve makine öğrenmesi modellerine etkilerini incelemek için kapsamlı bir performans değerlendirme yapılması planlanmıştır.

4. **Sonuçların Raporlanması**  
   Elde edilen sonuçlar ve bulgular, görselleştirmeler ve raporlarla desteklenmiştir.

---

#### Kullanılan Teknolojiler ve Kütüphaneler

- **Programlama Dili**: Python
- **Kütüphaneler**:
  - Veri İşleme: `pandas`, `numpy`
  - Görselleştirme: `matplotlib`, `seaborn`
  - Makine Öğrenmesi: `scikit-learn`, `RandomForestClassifier`, `KNNImputer`

---

#### Fonksiyonlar ve İşleyiş

Proje, eksik verilerin doldurulması ve analiz edilmesi için modüler bir yapıya sahiptir. Aşağıda temel fonksiyonların açıklamaları yer almaktadır:

1. **Sayısal Eksik Verilerin Doldurulması**  
   - Ortalama ile doldurma (`mean`): Eksik değerler sütun ortalamasıyla doldurulur.
   - Medyan ile doldurma (`median`): Eksik değerler sütun medyanıyla doldurulur.
   - En küçük komşu yöntemi (`KNN`): KNN algoritması kullanılarak eksik değerler tahmin edilir.
   - Tahmine dayalı doldurma: Bir regresyon modeli eğitilerek eksik değerler tahmin edilir.

2. **Kategorik Eksik Verilerin Doldurulması**  
   - Mod ile doldurma: Eksik değerler sütunun en sık görülen değeriyle doldurulur.
   - "Bilinmiyor" etiketi: Eksik değerler "Bilinmiyor" etiketiyle doldurulur.
   - Tahmine dayalı doldurma: Random Forest algoritmasıyla eksik değerler tahmin edilir.

3. **Veri Seti Yönetimi**  
   - Her eksik değer doldurma yöntemi için ayrı veri setleri oluşturulur.
   - Farklı yöntem kombinasyonlarını değerlendirmek üzere veri setleri bir listeye kaydedilir.

4. **Makine Öğrenmesi Modelleri**  
   Kodda, eksik veri doldurma yöntemlerinin sonuçlarını değerlendirmek için çeşitli modeller kullanılabilir. Modeller:
   - Doğrusal Regresyon
   - Rastgele Orman
   - Destek Vektör Regresyonu (SVR)

---

#### Çıktılar ve Değerlendirme

Proje çalıştırıldığında:
- Farklı doldurma yöntemleriyle oluşturulmuş veri setleri `final_imputed_data_sets` listesinde saklanır.
- Her veri seti üzerinde modelleme yapılabilir ve sonuçlar karşılaştırılabilir.

---

#### Sertifika

![image](https://github.com/user-attachments/assets/fff86f6d-93de-4d4d-b97d-ffe8017a85a3)

#### Youtube Linki
https://youtu.be/aKVu4DB_E90
