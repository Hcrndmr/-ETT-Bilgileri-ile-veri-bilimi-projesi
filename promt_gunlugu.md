
# Proje Prompt Günlüğü (Prompt Log)

Bu günlük, projenin geliştirilmesi esnasında yapay zeka asistanına verilen önemli komutları ve alınan sonuçları kronolojik sırayla içermektedir.

### 📌 1. Adım: Veri Yükleme ve Temizleme
* **Kullanım Amacı:** Veri setini doğru tiplere dönüştürmek ve aykırı değerleri temizlemek.
* **Gönderilen Prompt:**
    > "Elimde İBB toplu taşıma veri seti şeması var. Pandas kullanarak veri setini yükleyen, `transition_date` alanını datetime formatına, `transition_hour` alanını integer'a çeviren bir kod yazar mısın? Ayrıca `number_of_passage` ve `number_of_passenger` sütunlarındaki eksik değerleri 0 ile doldursun ve IQR yöntemiyle yolcu sayısındaki aşırı uç değerleri (outliers) temizlesin. Her satırı yorum satırıyla açıkla."
* **Alınan Sonuç:** Tip dönüşümleri tamamlandı, IQR filtresiyle hatalı veri girişleri temizlendi.

---

### 📌 2. Adım: Keşifsel Veri Analizi (EDA) ve Araştırma Soruları
* **Kullanım Amacı:** Belirlenen 3 araştırma sorusuna yönelik 4 farklı grafik türü üretmek.
* **Gönderilen Prompt:**
    > "Yukarıdaki İBB veri seti için şu 3 araştırma sorusunu yanıtlamak istiyorum: 1- Günün hangi saatlerinde yoğunluk zirve yapıyor? 2- En çok tercih edilen ulaşım ve transfer türü hangisi? 3- Kart türlerine göre yolculuk dağılımları nasıl? Bu soruları yanıtlamak için Seaborn ve Matplotlib kullanarak Line Plot, Bar Plot, Pie Chart ve Boxplot içeren 4 farklı görselleştirme kodu yazar mısın?"
* **Alınan Sonuç:** Saatlik yoğunluk çizgisi, ulaşım türü bar grafiği, aktarma oranları pastası ve kart türü kutu grafikleri başarıyla oluşturuldu.

---

### 📌 3. Adım: Modelleme (K-Means Kümeleme)
* **Kullanım Amacı:** Saatleri ve yolcu yoğunluklarını yapılandırılmamış şekilde gruplamak.
* **Gönderilen Prompt:**
    > "İBB toplu taşıma veri setiindeki `transition_hour`, `number_of_passage` ve `number_of_passenger` özelliklerini (features) kullanarak saatleri ve yoğunlukları K-Means algoritması ile 3 farklı yoğunluk kümesine (Sakin, Orta, Yoğun) ayıran bir Scikit-Learn kodu yazar mısın? Modeli kurmadan önce StandardScaler ile veriyi ölçeklendir (scale) ve sonuçları bir scatter plot üzerinde görselleştir."
* **Alınan Sonuç:** İstanbul içi "Yoğun-Orta-Sakin" saat/bölge kırılımlarını gösteren K-Means modeli kuruldu ve scatter plot ile görselleştirildi.
