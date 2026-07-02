
# Proje Prompt Günlüğü (Prompt Log)

Bu günlük, projenin geliştirilmesi esnasında yapay zeka asistanına verilen önemli komutları ve alınan sonuçları kronolojik sırayla içermektedir.

Prompt 1:
Elimde İBB toplu taşıma veri seti şeması var. Pandas kullanarak veri setini yükleyen, transition_date alanını datetime formatına, transition_hour alanını integer'a çeviren bir kod yazar mısın? Ayrıca number_of_passage ve number_of_passenger sütunlarındaki eksik değerleri 0 ile doldursun ve IQR yöntemiyle yolcu sayısındaki aşırı uç değerleri (outliers) temizlesin. Her satırı yorum satırıyla açıkla.
***Başlangıç aşaması***

prompt 2:
Yukarıdaki İBB veri seti için şu 3 araştırma sorusunu yanıtlamak istiyorum: 1- Günün hangi saatlerinde yoğunluk zirve yapıyor? 2- En çok tercih edilen ulaşım ve transfer türü hangisi? 3- Kart türlerine göre yolculuk dağılımları nasıl? Bu soruları yanıtlamak için Seaborn ve Matplotlib kullanarak Line Plot, Bar Plot, Pie Chart ve Boxplot içeren 4 farklı görselleştirme kodu yazar mısın?
***İncelenen soruları yazdım***

prompt 3:
yazdığım kodu nasıl çalıştıracağım
***python ile yazdım ve visual studio ortamında çalıştıramadım. Aldığım hataları yazdım ve visual studio AI ile birlikte sıfırdan jupyter dosyası oluşturdum***

prompt 4:
S C:\Users\hicra\OneDrive\Masaüstü\veri ödevi> python analiz.py
Traceback (most recent call last):
  File "C:\Users\hicra\OneDrive\Masaüstü\veri ödevi\analiz.py", line 1, in <module>
    import matplotlib.pyplot as plt
ModuleNotFoundError: No module named 'matplotlib'
PS C:\Users\hicra\OneDrive\Masaüstü\veri ödevi> 

prompt 5:
Python Pandas kullanarak veri.csv isimli bir İBB toplu taşıma veri setini yükleyen bir kod yazar mısın? Veri şemasındaki transition_date alanını datetime formatına, transition_hour alanını integer'a çevirsin. number_of_passage ve number_of_passenger sütunlarındaki eksik değerleri (NaN) 0 ile doldursun ve IQR yöntemiyle yolcu sayısındaki aykırı değerleri (outliers) temizlesin. Kod bloklarındaki her satırı yorum satırıyla açıkla.
***aykırı değerler temizlenir***

prompt 6:
yalnız ben bütün kodu python uzantılı dosyaya yazdım jupyter nootbooka nasıl çeviririm
***hatamı yazdım***

prompt 7:
Extension 'vscode.ipynb' is not known or not activated. View Jupyter log for further details.
***visual studio code un bana ilettiği hataları yazdım***


prompt 8:
tamam sil baştan yapalım şunu
***tekrardan jupyter dosyası açarak projeye devam ettim. Yukarıda aldığım çıktıları jupyter dosyasına ekledim***


prompt 9:
şimdi bu jpynb uzantılı çalışmayı nasıl çalıştıracam
***jupyter dosyasını nasıl çalıştıracağımı yapay zekaya sordum***

***Bu noktadan sonra koddaki hataları düzeltmek için prompt yazmaya devam ettim***
