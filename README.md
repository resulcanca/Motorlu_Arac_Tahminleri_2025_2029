#  Türkiye ve İstanbul Motorlu Kara Taşıtı Kayıt Tahmin Projesi (2025-2029)

Bu proje, T.C. İçişleri Bakanlığı tarafından trafiğe yeni kaydedilen motorlu kara taşıtlarının yıllara ve yakıt türlerine göre dağılımını analiz ederek, önümüzdeki 5 yıla dair (2025-2029) tahminler üretmeyi amaçlamaktadır.

## 🚀 Proje Amacı

Türkiye'nin ve İstanbul'un hızla değişen araç parkı dinamiklerini, özellikle elektrikli ve hibrit araçlardaki yükselişi ve geleneksel yakıtlardaki (Dizel, LPG) düşüşü kantitatif verilerle ortaya koymak ve geleceğe yönelik stratejik öngörüler sağlamaktır.

## 📊 Veri Seti

* **Kaynak:** İstanbul Büyükşehir Belediyesi Açık Veri Portalı (İBB)
    * **Veri Seti Linki:** [https://data.ibb.gov.tr/dataset/yillara-gore-trafige-kaydi-yapilan-motorlu-kara-tasit-sayisi](https://data.ibb.gov.tr/dataset/yillara-gore-trafige-kaydi-yapilan-motorlu-kara-tasit-sayisi)
* **Lisans:** İstanbul Büyükşehir Belediyesi Açık Veri Lisansı (Genellikle Kaynak Gösterme zorunluluğu esasına dayanır, verinin ticari ve ticari olmayan her amaçla kullanımına izin verir).
* **Kırılım:** İl (İstanbul/Türkiye) ve Yakıt Türü (Benzinli, Dizel, Hibrit, Elektrik, LPG).
* **Tarih Aralığı:** 2020 - 2024.

## 🧠 Kullanılan Metodoloji ve Model

Kısıtlı zaman serisi verisi (5 yıllık) göz önüne alınarak, her bir yakıt türü/lokasyon serisi için ayrı ayrı **Doğrusal Regresyon (Linear Regression)** modeli kullanılmıştır.

### 🛠️ Teknik Detaylar

| Bileşen | Detay |
| :--- | :--- |
| **Geliştirme Ortamı** | Jupyter Notebook|
| **Programlama Dili** | Python |
| **Temel Kütüphaneler** | `pandas`, `numpy`, `matplotlib`, `scikit-learn` (`LinearRegression`) |
| **Çıktı** | `Motorlu_Arac_Tahminleri_2025_2029.csv` (Tahmini sonuçlar) |

## 🚀 Projeyi Çalıştırma

1.  Bu repoyu klonlayın.
2.  Gerekli kütüphaneleri yükleyin: `pip install pandas numpy scikit-learn matplotlib`
3.  Jupyter dosyasını çalıştırın.
4.  Tahmin sonuçları, projenin ana dizininde **`Motorlu_Arac_Tahminleri_2025_2029.csv`** olarak kaydedilecektir.
