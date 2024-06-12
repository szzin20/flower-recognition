# Ikhtiar Oktafio Wibowo 21102101 - Firman Adi Ramadhan 21102083


# Flower Recognition using CNN with Keras

Repositori ini berisi proyek untuk mengenali berbagai spesies bunga menggunakan Convolutional Neural Network (CNN) yang diimplementasikan dengan Keras. Proyek ini terinspirasi dan berdasarkan pada notebook Kaggle yang dibuat oleh Raj Mehra.

## Daftar Isi
- [Ringkasan](#ringkasan)
- [Dataset](#dataset)
- [Instalasi](#instalasi)
- [Arsitektur Model](#arsitektur-model)
- [Pelatihan](#pelatihan)
- [Evaluasi](#evaluasi)
- [Hasil](#hasil)

## Ringkasan

Tujuan dari proyek ini adalah membangun model deep learning untuk mengklasifikasikan gambar bunga ke dalam kategori yang berbeda. Proyek ini menggunakan Convolutional Neural Network (CNN) untuk melakukan klasifikasi gambar, dengan memanfaatkan Keras untuk membangun dan melatih model.

## Dataset

Dataset yang digunakan dalam proyek ini adalah Flowers Recognition dataset dari Kaggle. Dataset ini berisi gambar bunga yang dikategorikan ke dalam lima kelas berbeda:
- Daisy
- Dandelion
- Rose
- Sunflower
- Tulip

Dataset dapat diunduh dari [sini](https://drive.google.com/drive/folders/1k1YNiHkt3kLcHGwfUj2nLX1DZEs9mCzr?usp=sharing).

## Instalasi

Untuk menjalankan proyek ini, Anda perlu menginstal Python beserta pustaka-pustaka yang diperlukan. Anda dapat menginstal pustaka-pustaka yang dibutuhkan menggunakan `pip`.

```bash
pip install -r requirements.txt
The requirements.txt file includes:

tensorflow
keras
numpy
pandas
matplotlib
scikit-learn

## **Arsitektur Model**
Model CNN yang digunakan dalam proyek ini terdiri dari lapisan-lapisan berikut:

Lapisan konvolusional dengan aktivasi ReLU dan MaxPooling
Lapisan fully connected (Dense) dengan Dropout untuk regularisasi
Lapisan Softmax untuk klasifikasi output
Berikut adalah ringkasan arsitektur model:
Layer (type)                 Output Shape              Param #
=================================================================
conv2d (Conv2D)              (None, 128, 128, 32)      896
...
dense (Dense)                (None, 512)               131584
...
dense_1 (Dense)              (None, 5)                 2565
=================================================================
Total params: 2,846,213
Trainable params: 2,846,213
Non-trainable params: 0

## **Pelatihan**
Model dilatih menggunakan langkah-langkah berikut:

Augmentasi Data: Untuk mencegah overfitting dan membuat model lebih robust, teknik augmentasi data seperti rotasi, zoom, dan flipping horizontal diterapkan.
Kompilasi: Model dikompilasi menggunakan optimizer Adam dan fungsi loss categorical cross-entropy.
Pelatihan: Model dilatih pada dataset pelatihan untuk sejumlah epoch tertentu, dengan validasi split untuk memantau kinerja.

**## Evaluasi**
![image](https://github.com/szzin20/flower-recognition/assets/92289030/342f9546-a403-4ca3-a3a6-10fa14a792dc)
![image](https://github.com/szzin20/flower-recognition/assets/92289030/8f1c3bf1-bd76-4203-9025-6837258d1e8e)


**## Hasil**
Model akhir mencapai akurasi tinggi pada dataset uji, menunjukkan efektivitasnya dalam mengklasifikasikan berbagai spesies bunga. Contoh hasil dibawah ini :
![image](https://github.com/szzin20/flower-recognition/assets/92289030/a486a78f-748e-4c93-9134-50154265748a)
![image](https://github.com/szzin20/flower-recognition/assets/92289030/48036037-d1be-493b-bc46-8caf29b583c2)





