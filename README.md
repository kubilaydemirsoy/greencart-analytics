# 🌍 GreenCart Analytics: Sürdürülebilir E-Ticaret ve Akıllı Lojistik

## 📝 Proje Hakkında
GreenCart Analytics, e-ticaret satış verilerini klasik "kâr optimizasyonu" yerine **çevresel sürdürülebilirlik ve karbon ayak izi minimizasyonu** hedefiyle inceleyen kapsamlı bir veri bilimi projesidir. Bu proje; gereksiz lojistik hareketliliğini, dürtüsel alışveriş kaynaklı iade atıklarını ve fazla üretimden doğan stok israfını makine öğrenmesi algoritmalarıyla tespit edip engellemeyi amaçlar.

## 🎯 Temel Hedefler ve İş Çıktıları (Actionable Insights)
* **Karbon İsrafı Şampiyonları:** İade oranı %100'ü aşan ve çifte kargo emisyonu yaratan problemli ürünlerin tespiti.
* **Küresel Lojistik Optimizasyonu:** İngiltere'den Avustralya gibi uzak rotalara giden tekil kargoların yarattığı devasa karbon ayak izinin 3 boyutlu küresel haritalanması.
* **Dürtüsel Alışverişin Engellenmesi:** Salı ve Perşembe sabah 11:00 ile Pazartesi 13:00'te zirve yapan hatalı/iade edilecek sipariş saatlerinin Isı Haritası (Heatmap) ile tespiti.
* **Sıfır Atık Depo Yönetimi:** Geleneksel "stokta bulunsun" mantığı yerine, veri güdümlü üst limitler belirleyerek çürüyen/atığa dönüşen envanter maliyetlerinin sıfırlanması.

## 🧠 Geliştirilen Analitik Modeller ve Algoritmalar
* **Green RFM Segmentasyonu:** Müşterileri ne kadar para harcadıklarına göre değil; iade (kargo israfı) sıklıklarına ve sepet verimliliklerine göre *Standart, Çevre Dostu* ve *Riskli (Yüksek Karbon)* olarak gruplandıran özgün RFM yaklaşımı.
* **Apriori Algoritması ile Sepet Birleştirme:** Alman pazarındaki alışveriş kalıplarını analiz ederek "Birlikte Alınan" ürünlerin tespiti (Örn: Red Retrospot Çanta alanların %84 ihtimalle Woodland Çanta alması). Bu kural sayesinde ürünler tek kargoda birleştirilerek lojistik emisyonu yarı yarıya düşürülmüştür.
* **Prophet ile Zaman Serisi ve Talep Tahmini:** Gelecek 90 günün optimum günlük talep miktarının %95 güven aralığı ile tahmin edilmesi ve üretim bantları için kesin "Üst Sınır (yhat_upper)" kotalarının belirlenmesi.
* **Ağ Analizi (Network Graph):** Birlikte satın alınan ve tek kargoda birleştirilmeye en uygun kilit (Hub) ürün kümelerinin interaktif tespiti.

## 🛠️ Kullanılan Teknolojiler
* **Programlama Dili:** Python
* **Veri İşleme:** Pandas, NumPy
* **Makine Öğrenmesi & İstatistik:** Facebook Prophet (Zaman Serisi), MLxtend (Apriori Algoritması)
* **Ağ Analizi:** NetworkX
* **Veri Görselleştirme:** Plotly (İnteraktif 3D Küre ve Zaman Çizelgeleri), Seaborn, Matplotlib, Missingno

## 🚀 Kurulum ve Çalıştırma
1. Bu repoyu bilgisayarınıza klonlayın:
   `git clone https://github.com/kullaniciadi/greencart-analytics.git`
2. Gerekli Python kütüphanelerini yükleyin:
   `pip install pandas numpy matplotlib seaborn plotly missingno prophet mlxtend networkx`
3. Veri setini (`ecommerce.csv`) ana dizine ekleyin.
4. `greencartanalyticsders.ipynb` dosyasını Jupyter Notebook veya Google Colab üzerinde açarak hücreleri sırasıyla çalıştırın.
