# Predicting Electrical Grid Stability using Machine Learning

## Latar Belakang

Jaringan listrik (Electrical Grid) merupakan infrastruktur yang sangat krusial dan diperlukan monitoring secara kontinyu untuk menjaga kestabilan sistem kelistrikan. Kestabilan jaringan dapat dipengaruhi oleh beberapa faktor diantaranya adalah keseimbangan antara kebutuhan energi dan pasokan energi, frekuensi deviasi, dan elastisitas harga listrik. Biasanya untuk menjaga kestabilan energi masih dilakukan secara manual oleh grid operators, yang mana dapat memakan waktu dan kurang efisien. Dalam beberapa tahun belakangan ini, terdapat terobosan untuk mengembangkan sistem otomatis yang dapat memprediksi perubahan dari kestabilan jaringan listrik, disinlah peran dari machine learning untuk menghasilkan prediksi dari potensi terjadinya perubahan kestabilan energi.

Pada kontek ini, dataset yang digunakan berasal dari Electrical Grid Stability Simulated Data Set dari UCI Machine Learning Repository. Dari dataset ini kita dapat menganalisa hubungan antara input variables seperti nominal power, reaction time, dan price lasticity dengan kestabilan jaringan listrik. Hasil dari analisis ini dapat digunakan untuk mengembangkan sistem yang lebih akurat dan andal dalam memprediksi dan mengelola kestabilan jaringan secara real time.

Source: https://archive.ics.uci.edu/ml/datasets/Electrical+Grid+Stability+Simulated+Data+

![image.png](attachment:image.png)

## Tujuan
Tujuan utama dari projek ini adalah untuk mengembangkan machine learning model yang mampu memprediksi dengan akurat kestabilan jaringan listrik berdasarkan input variables di Electrical Grid Stability Simulated Data Set. Serta menjabarkan potensi kegunaan dari machine learning dalam memprediksi kestabilan grid, seperti meningkatkan effisiensi, mengurangi downtime, dan meningkatkan keandalan sistem.

## Metrik Evaluasi
Pada projek ini akan menggunakan ROC AUC sebagai metrik evaluasi, ROC AUC digunakan untuk mengevaluasi seberapa baik model mampu membedakan anatara sistem yang stabil dan tidak stabil berdasarkan variabel input yang diberikan. 

## Informasi Data Set

Dataset ini terdiri dari 11 atribut prediktif, 1 atribut non-prediktif (p1), dan 2 atribut label:

1. tau[x]: waktu reaksi peserta (real dalam rentang [0,5,10] detik). Tau1 - nilai untuk produsen listrik.
2. p[x]: daya nominal yang dikonsumsi(negatif)/dihasilkan(positif)(real). Untuk konsumen, rentangnya adalah [-0,5,-2]s^-2; p1 = abs(p2 + p3 + p4).
3. g[x]: koefisien (gamma) proporsional terhadap elastisitas harga (real dalam rentang [0,05,1]s^-1). g1 - nilai untuk produsen listrik.
4. stab: bagian riil maksimum dari akar persamaan karakteristik (jika positif - sistem tidak stabil secara linear)(real).
5. stabf: label stabilitas sistem (kategori: stabil/tidak stabil).
