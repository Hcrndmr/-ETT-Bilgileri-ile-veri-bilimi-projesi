# -ETT-Bilgileri-ile-veri-bilimi-projesi
İETT verileri alınarak İstanbul ilinde toplu taşıma ile ilgili sorular incelendi

Hicran Demir - 1306220039

# Projeyi Çalıştırma Talimatları

Bu projeyi yerel bilgisayarınızda veya her adımı doğrulamak için sıfırdan çalıştırmak için aşağıdaki adımları sırasıyla takip ediniz:

# 1. Projeyi Bilgisayarınıza İndirin
Öncelikle bu depoyu (repository) bilgisayarınıza klonlayın veya ZIP olarak indirip bir klasöre çıkartın:
```bash
git clone [https://github.com/](https://github.com/)[github-kullanici-adin]/ibb-toplu-tasima-veri-bilimi.git
cd ibb-toplu-tasima-veri-bilimi

# 2. Gerekli Kütüphaneleri Kurun
Projenin çalışması için gerekli olan tüm Python kütüphanelerini terminal veya komut satırı (CMD) üzerinden aşağıdaki komutla yükleyin:

Bash
pip install pandas numpy matplotlib seaborn scikit-learn ipykernel notebook

# 3. Veri Setini Yerleştirin
İBB Açık Veri Portalı'ndan indirdiğiniz veya proje için hazırlanan güncel toplu taşıma veri setini içeren CSV dosyasının adını ibb_toplu_tasima_veri_seti.csv olarak değiştirin.

Bu dosyayı, analiz.ipynb dosyasının bulunduğu kök dizine (aynı klasör içine) kopyalayın.

# 4. Jupyter Notebook'u Başlatın ve Çalıştırın
VS Code kullanıyorsanız doğrudan analiz.ipynb dosyasını açıp sağ üstten Python çekirdeğini (Kernel) seçerek çalıştırabilirsiniz. Eğer tarayıcı üzerinden çalıştırmak isterseniz terminale şu komutu yazın:

Bash
jupyter notebook
Açılan sekmede analiz.ipynb doshasına tıklayın ve yukarıdaki menüden "Run All" (Hepsini Çalıştır) butonuna basarak veri temizleme, EDA ve makine öğrenmesi adımlarının kronolojik olarak akmasını sağlayın.

Pandas & NumPy: Veri setinin yüklenmesi, eksik verilerin (NaN) doldurulması, veri tipi dönüşümleri ve IQR tabanlı aykırı değer temizliği işlemleri için kullanılmıştır.

Matplotlib & Seaborn: Projenin teknik gereksinimlerinde yer alan en az 4 farklı grafik türünün (Line Plot, Bar Plot, Pie Chart, Box Plot) ve model sonuçlarının yüksek kaliteli, Türkçe etiketli görselleştirmeleri için kullanılmıştır.

Scikit-Learn (sklearn): Verilerin K-Means modeline girmeden önce ölçeklendirilmesi (StandardScaler) ve saatlik yolcu trafiğinin 3 farklı yoğunluk kümesine ayrılması için kullanılmıştır.


### Lisans bilgileri: https://data.ibb.gov.tr/license
                      https://data.ibb.gov.tr/dataset/hourly-public-transport-data-set/resource/75e25417-36df-4822-8a18-578f0f7a584a
