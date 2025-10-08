# 5220411274 | Anandava Eka Buana Baskara
## Analisis Sentimen Twitter/X mengenai coin cryptocurrency SPX6900

### Deskripsi Proyek
SPX6900 (SPX) adalah memecoin yang diluncurkan pada Agustus 2023 sebagai parodi terhadap indeks S&P 500, dengan ambisi satir untuk mencapai kapitalisasi pasar sebesar $69 triliun. Setelah pengembang awal meninggalkan proyek, komunitas mengambil alih sepenuhnya, menjadikannya proyek yang sepenuhnya terdesentralisasi dan berbasis komunitas.
Token SPX memiliki total pasokan 1 miliar, dengan sekitar 930 juta token beredar. Sebagai memecoin, SPX tidak memiliki utilitas teknis yang signifikan, namun nilai dan daya tariknya berasal dari komunitas yang aktif dan narasi satir terhadap sistem keuangan tradisional.

### Tahapan Proses

1. **Pengumpulan Data (Crawling):**  
   Mengambil data tweet yang mengandung kata kunci `SPX6900` dalam rentang waktu 01-08-2025 sampai 01-10-2025 sejumlah 1500 data menggunakan crawler berbasis token autentikasi Twitter.
2 **Pembersihan Data (Case Folding)**
   - Menghapus URL, hashtag, mention, angka, dan karakter khusus.
   - Normalisasi teks (lowercase).
   - Tokenisasi kata.
3 **Melakukan sentimen analisis menggunakan lexicon VADER**
   lexicon VADER digunakan untuk menentukan emosi berbasis skor dengan acuan nilai positif, negatif dan netral,
   nilai positif didapatkan apabila skor >= 0,05, untuk negatif didapatkan bila skor <= -0,05, diantara itu netral.
4. **Melakukan visualisasi data terhadapat sentimen positif, negatif dan netral**
   Visualisasi ini digunakan untuk melihat hasil dari skor sentimen yang dihasilkan oleh lexicon VADER menggunakan seaborn.

## Hasil
1. Dataset Twitter bertema SPX6900 berhasil dibesihkan dan di proses dengan baik.
2. Sentimen tersebut dapat memberikan gambaran mengenai presepsi yang dimiliki pengguna x terhadap spx6900.

## Pengembangan
1. Melihat keterkaitan antara data aktual (chart) pada coin SPX6900 dengan sentimen yang terjadi berdasarkan baris created_at.
