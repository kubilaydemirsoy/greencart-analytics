# 🛒 Green Cart Analytics: E-Ticaret Veri Analizi ve Zaman Serisi Tahmini

Bu proje, gerçek dünya e-ticaret işlem verileri kullanılarak gerçekleştirilen Keşifçi Veri Analizi (EDA) ve Zaman Serisi Tahmini (Forecasting) çalışmalarını içermektedir. Temel amaç, müşteri satın alma kalıplarını ortaya çıkarmak, eksik verileri işlemek, satış trendlerini görselleştirmek ve gelişmiş tahmin modelleri kullanarak gelecekteki satışları öngörmektir.

## 📊 Proje Özeti
Bu çalışmada, e-ticaret veri seti üzerinden eyleme dönüştürülebilir içgörüler elde edilmiştir. Çalışma akışı şu adımları içermektedir:
* **Veri Temizleme ve Ön İşleme:** Eksik değerlerin ele alınması ve tarih formatlarının düzenlenmesi.
* **Keşifçi Veri Analizi (EDA):** Satış trendlerinin, müşteri coğrafi dağılımının ve en çok satan ürünlerin görselleştirilmesi.
* **Zaman Serisi Tahmini:** Geçmiş verilere dayanarak gelecekteki satış trendlerini tahmin etmek için **Prophet** modelinin kullanılması.

## 🛠️ Kullanılan Teknolojiler ve Kütüphaneler
Proje, Google Colab ortamında Python kullanılarak geliştirilmiştir. Öne çıkan kütüphaneler şunlardır:
* **Veri İşleme:** `pandas`, `numpy`
* **Veri Görselleştirme:** `matplotlib`, `seaborn`, `plotly.express`, `missingno`
* **Zaman Serisi Tahmini:** `prophet`

## 📂 Veri Seti Hakkında
Kullanılan veri seti, İngiltere merkezli çevrimiçi bir perakende şirketinin uluslararası işlemlerini içermektedir. 
**Not:** Veri seti boyutu büyük olduğu için GitHub'a **`ecommerce.rar`** olarak sıkıştırılarak yüklenmiştir.

* **InvoiceNo:** Fatura numarası. Her işleme atanan 6 haneli benzersiz numara.
* **StockCode:** Ürün (stok) kodu.
* **Description:** Ürün adı.
* **Quantity:** Her işlemdeki ürün miktarı.
* **InvoiceDate:** Fatura tarihi ve saati.
* **UnitPrice:** Birim fiyat. Ürünün sterlin cinsinden fiyatı.
* **CustomerID:** Müşteri numarası. Her müşteriye atanan 5 haneli benzersiz numara.
* **Country:** Ülke adı. Müşterinin ikamet ettiği ülke.

## 🚀 Projeyi Çalıştırma Adımları
Projeyi kendi bilgisayarınızda veya Colab üzerinde çalıştırmak için aşağıdaki adımları izleyin:

1. Bu depoyu (repository) yerel makinenize klonlayın:
   ```bash
   git clone [https://github.com/kullanici-adiniz/greencart-analytics.git](https://github.com/kullanici-adiniz/greencart-analytics.git)
2. Depo içindeki ecommerce.rar dosyasını aynı klasör dizinine çıkartın (WinRAR, 7-Zip vb. kullanarak). Çıkarma işlemi sonucunda ecommerce.csv dosyasını elde edeceksiniz.

3. greencartanalytics.ipynb dosyasını Google Colab veya Jupyter Notebook üzerinden açın.

4. Çıkarttığınız ecommerce.csv dosyasının notebook ile aynı dizinde olduğundan emin olun (veya Colab kullanıyorsanız oturumunuza yükleyin).

5. Analizleri ve tahminleri görmek için hücreleri sırasıyla çalıştırın.
