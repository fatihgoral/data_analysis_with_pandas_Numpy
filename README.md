# Veri Ön İşleme, EDA ve Özellik Mühendisliği Çalışmaları

Bu depo, Makine Öğrenmesi modelleri kurulmadan önce verinin nasıl hazırlanması, temizlenmesi ve analiz edilmesi gerektiğine dair çeşitli uygulamaları içermektedir. İçerisinde veri dengeleme, kategorik değişken kodlama ve farklı veri setleri üzerinde Keşifsel Veri Analizi (EDA) adımlarını barındıran Jupyter Notebook dosyaları bulunmaktadır.

## 📂 İçerik ve Dosya Yapısı

Proje içerisindeki her bir notebook, veri biliminin farklı bir temel konseptine odaklanmaktadır:

* **`1-BalancingData.ipynb`**: Dengesiz veri setleri (Imbalanced Data) üzerinde çalışmalar. Sentetik olarak üretilen dengesiz bir veri setinde (900'e 100 oranlı) azınlık sınıfını çoğaltma (Oversampling) gibi veri dengeleme teknikleri uygulanmıştır.
* **`Encoding.ipynb`**: Kategorik verilerin sayısal formata dönüştürülmesi. Popüler `Titanic` veri seti üzerinden `LabelEncoder` ve `OrdinalEncoder` (örneğin; "Third", "Second", "First" sınıflarının hiyerarşik kodlanması) kullanımları gösterilmiştir.
* **`BoxPlot.ipynb`**: Veri görselleştirme ve aykırı değer (outlier) analizi. Yine `Titanic` veri seti kullanılarak yolcu yaşları ve bilet fiyatlarının (`fare`) sınıflara göre dağılımı, logaritmik ölçekleme teknikleri kullanılarak Kutu Grafikleri (Box Plots) ile incelenmiştir.
* **`1-FeatureEngineriingEDA.ipynb`**: `Google Play Store` verisi üzerinde uçtan uca veri temizleme, metin verilerini sayısal verilere dönüştürme ve yeni özellikler (feature) üretme süreçlerini içerir.
* **`EDAexercise_start.ipynb`**: `WineQT.csv` (Şarap Kalitesi) veri seti üzerinde özelliklerin dağılımlarını anlamak için yapılan veri keşfi analizidir.

## 📊 Görselleştirmeler
Depo içerisinde analiz süreçlerinden elde edilen dağılım, korelasyon ve kutu grafiklerine ait çeşitli `.png` formatında çıktı görselleri de yer almaktadır. Bu görseller verideki desenleri ve aykırılıkları anlamak için kullanılmıştır.

## 🛠️ Kullanılan Teknolojiler

Bu çalışmalarda aşağıdaki Python kütüphaneleri aktif olarak kullanılmıştır:
* **Veri Manipülasyonu:** `pandas`, `numpy`
* **Veri Görselleştirme:** `matplotlib.pyplot`, `seaborn`
* **Makine Öğrenmesi Araçları:** `scikit-learn` (`OrdinalEncoder`, `LabelEncoder` vb.)

## ⚙️ Kurulum ve Kullanım

Çalışmaları kendi ortamınızda test etmek için:

1.  Python ortamınıza gerekli kütüphaneleri kurun:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
2.  Kullanılan veri setlerinin (`17-googleplaystore.csv`, `WineQT.csv` vb.) ilgili notebook dosyaları ile aynı dizinde olduğundan emin olun. (Titanic veri seti Seaborn kütüphanesi üzerinden otomatik çekilmektedir.)
3.  Jupyter Notebook'u başlatarak dilediğiniz analiz dosyasını çalıştırın.
