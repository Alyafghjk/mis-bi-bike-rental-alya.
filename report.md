# Bike Rental Business Analytics Report

## 1. Business Problem
Analisis ini bertujuan untuk mengevaluasi faktor-faktor yang mempengaruhi permintaan penyewaan sepeda, memahami perilaku pelanggan, serta membangun model prediktif untuk mengoptimalkan operasional armada dan strategi bisnis perusahaan.

## 2. Dataset
Dataset yang digunakan adalah data harian penyewaan sepeda tahun 2011–2012, mencakup variabel kalender (musim, hari kerja, libur), kondisi cuaca (suhu, kelembapan, angin), dan data transaksi (pengguna casual, registered, dan total).

## 3. Descriptive Analytics
Tujuan: Memahami aktivitas bisnis yang sudah terjadi.
![Descriptive Analytics](images/descriptive.png)
* Temuan: Puncak permintaan terjadi pada musim panas/gugur. Pengguna Registered mendominasi transaksi harian.

## 4. Diagnostic Analytics
Tujuan: Menganalisis mengapa terjadi fluktuasi permintaan.
![Diagnostic Analytics](images/diagnostic.png)
* Temuan: Kondisi cuaca (weathersit) dan status hari kerja (workingday) berkaitan erat dengan fluktuasi volume penyewaan harian.

## 5. Clustering dan Hidden Pattern
Tujuan: Mengidentifikasi kelompok hari dengan karakteristik serupa.
![Clustering](images/clustering.png)
* Interpretasi: Cluster 0 (Kondisi buruk), Cluster 1 (Kondisi ideal), Cluster 2 (Kondisi normal). 
* Hidden Pattern: Pengguna Casual jauh lebih sensitif terhadap perubahan cuaca dibandingkan pengguna Registered.

## 6. Predictive Analytics
Tujuan: Memprediksi permintaan (High vs Low Demand).
![Confusion Matrix](images/confusion_matrix.png)
* Hasil: Model Decision Tree dengan akurasi tinggi mampu membedakan tingkat permintaan berdasarkan faktor lingkungan tanpa data leakage.

## 7. Prescriptive Recommendation
1. Manajemen armada dinamis berbasis cuaca.
2. Penjadwalan maintenance pada hari "Low Demand".
3. Kampanye konversi member bagi pengguna Casual.

## 8. Conclusion
Analisis ini membuktikan bahwa integrasi data historis dengan *Machine Learning* sangat krusial dalam pengambilan keputusan operasional untuk meminimalkan biaya dan memaksimalkan pendapatan..
