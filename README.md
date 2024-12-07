# sentimen-analisis-studi1

# Klasifikasi Sentimen Analisis Scraping Youtube dengan Algoritma KNN

## Deskripsi

Program ini dirancang untuk melakukan analisis sentimen pada komentar YouTube yang dikumpulkan melalui proses scraping. Program ini memanfaatkan algoritma K-Nearest Neighbors (KNN) untuk mengklasifikasikan sentimen dan TextBlob untuk melakukan pelabelan sentimen awal. Berdasarkan pengujian, model KNN yang digunakan mencapai akurasi sebesar 81.82%.

## Cara Kerja

Program ini bekerja melalui serangkaian tahapan:

1. **Scraping Komentar YouTube:** Program ini menggunakan YouTube Data API untuk mengambil komentar dari video YouTube tertentu.
2. **Preprocessing Data:** Komentar yang telah dikumpulkan kemudian diproses, termasuk:
    - **Case Folding:** Mengubah semua teks menjadi huruf kecil.
    - **Pembersihan Karakter Khusus:** Menghapus tanda baca dan karakter khusus yang tidak diperlukan.
    - **Tokenisasi:** Memecah teks menjadi kata-kata individual (token).
3. **Pelabelan Sentimen:** TextBlob digunakan untuk menganalisis polaritas setiap komentar dan memberikan label sentimen awal (positif, negatif, atau netral).
4. **Ekstraksi Fitur:** Program ini menggunakan TF-IDF (Term Frequency-Inverse Document Frequency) untuk mengekstrak fitur penting dari teks komentar.
5. **Pelatihan Model KNN:** Model KNN dilatih menggunakan data komentar yang telah dilabeli dan diekstrak fiturnya.
6. **Evaluasi Model:** Kinerja model dievaluasi menggunakan metrik seperti akurasi, presisi, recall, dan F1-score.
7. **Visualisasi:** Confusion matrix digunakan untuk memvisualisasikan hasil evaluasi model.
8. **Penyimpanan Model:** Model KNN dan vectorizer TF-IDF disimpan untuk penggunaan selanjutnya.

## Teknologi yang Digunakan

- **Python:** Bahasa pemrograman utama yang digunakan.
- **YouTube Data API:** Untuk mengakses dan mengambil data komentar YouTube.
- **TextBlob:** Untuk pelabelan sentimen awal.
- **Scikit-learn:** Untuk algoritma KNN, TF-IDF, dan evaluasi model.
- **NLTK:** Untuk preprocessing teks.
- **Pandas:** Untuk manipulasi dan analisis data.


## Cara Menjalankan Program

1. Pastikan Anda telah menginstal semua library yang diperlukan.
2. Masukkan API Key YouTube Anda.
3. Masukkan URL video YouTube yang ingin dianalisis.
4. Jalankan program.

## Kontribusi

Kontribusi sangat diapresiasi! Jika Anda menemukan bug atau memiliki saran untuk perbaikan, silakan buka issue atau pull request.
