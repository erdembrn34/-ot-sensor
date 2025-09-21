# IoT Sensor Data Analysis

Bu proje, sahte IoT sensör verileri üreterek veri analizi, veri kalitesi kontrolleri ve görselleştirme süreçlerini içermektedir. Amaç, IoT veri akışını simüle etmek ve temel veri işleme ve analiz adımlarını göstermek.

---

## 📂 Proje Yapısı

iot-sensor-project/
│
├─ data/
│ ├─ sensor_data.parquet # Tüm sensör verileri
│ ├─ anomalies.csv # Tespit edilen anomaliler
│ ├─ summary_report.html # Sensör bazlı özet analiz
│ └─ data_quality_report.html # Veri kalitesi raporu
│
├─ notebooks/
│ └─ iot_sensor_analysis.ipynb # Jupyter Notebook

📝 Proje Adımları

1.Sahte IoT Verisi Üretimi:
Sensör ID, sıcaklık, nem, basınç, CO2, ışık, batarya ve titreşim verileri oluşturulur.

2.Eksik Veri ve Temizleme:
Eksik değerler sensör bazlı ortalama ile doldurulur.

3.Anomali / Outlier Detection:
Z-score yöntemi ile sıcaklık anomalileri tespit edilir.

4.Batch Analizi & Rolling Metrics:
Sensör bazlı ortalama, minimum, maksimum ve rolling ortalamalar hesaplanır.

5.Veri Kalitesi Kontrolleri:
Eksik veri ve outlier sayıları raporlanır.

6.Veri Gölü / Parquet Kaydetme:
Veriler Parquet formatında saklanır, raporlar HTML ve CSV olarak kaydedilir.

7.Görselleştirme:

Matplotlib ile sensörlerin zaman serisi grafikleri

Plotly ile interaktif grafikler oluşturulur

8.HTML Raporlama:

summary_report.html → Sensör bazlı özet analiz

data_quality_report.html → Veri kalitesi raporu

🚀 Notlar

Bu proje sahte veri ile çalışmaktadır; gerçek IoT cihazları ile entegrasyon için veri alma ve bağlantı katmanı eklenmelidir.

Veriler Parquet formatında saklandığı için büyük veri senaryolarında ölçeklenebilir.

Anomali tespiti ve veri kalitesi raporları, sensör izleme ve bakım süreçlerinde kullanılabilir.
