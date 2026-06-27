# 📊 Analisis Sentimen Berbasis IndoBERT pada Berita Saham Indonesia

Repositori ini berisi implementasi lengkap proyek analisis sentimen menggunakan **IndoBERT** dari framework **[IndoNLU](https://github.com/IndoNLP/indonlu)**. Penelitian ini berfokus pada klasifikasi judul berita saham Indonesia dari **CNBC Indonesia** ke dalam sentimen **positif**, **netral**, atau **negatif**.

---

## 📁 Struktur Repositori

Repositori terdiri dari dua folder utama:

- `Dataset/`: Berisi dataset asli dan dataset yang telah dibagi (rasio 90:10, 80:20, 70:30), serta file CSV hasil pra-pemrosesan.
- `Codes/`: Berisi notebook Jupyter untuk pra-pemrosesan dan analisis sentimen.

---

## 📚 Ringkasan

- **Model**: IndoBERT-Large (`indobenchmark/indobert-large-p2`)
- **Framework**: IndoNLU
- **Ukuran dataset**: 9.819 judul berita
- **Kelas sentimen**: `positif`, `netral`, `negatif`
- **Sumber data**: CNBC Indonesia Market section (2024–2025)

Repositori ini mendukung eksperimen yang dapat direproduksi menggunakan stratified shuffle split serta berbagai skenario learning rate dan konfigurasi early stopping.

---

## 🧪 Fitur Utama

- ✅ Fine-tuning IndoBERT untuk klasifikasi teks Bahasa Indonesia
- ✅ Pelabelan sentimen manual pada judul berita saham
- ✅ Optimasi pembagian dataset menggunakan **Jaccard Similarity**
- ✅ Empat konfigurasi learning rate (2e-5, 3e-5, 2e-6, 3e-6)
- ✅ Kontrol pelatihan dengan early stopping
- ✅ Metrik evaluasi: Akurasi, Presisi, Recall, F1-score
- ✅ Reproduksibilitas dengan random seed dan pembagian data terkontrol

---

## 🚀 Mulai Cepat

Proyek ini direkomendasikan untuk dijalankan menggunakan **Google Colab**.

### ▶️ Buka di Google Colab

Anda dapat mengunggah repositori ini ke Google Drive atau GitHub, lalu buka notebook berikut:

- `Codes/preprocessing.ipynb`: Untuk membersihkan dan tokenisasi dataset
- `Codes/sentiment-analyzer.ipynb`: Untuk fine-tuning IndoBERT dan evaluasi

Perbarui path dan konfigurasi sesuai kebutuhan di dalam script.

---

## 📦 Akses Dataset

Dataset lengkap yang digunakan dalam proyek ini tersedia di Kaggle:  
🔗 [Kaggle Dataset: Sentiment-Labeled Stock News Headlines](https://www.kaggle.com/datasets/triagungj/cnbc-indonesia-stock-news-sentiment-dataset/data)

---

## 🙏 Ucapan Terima Kasih

Penelitian ini memanfaatkan:

- Repositori IndoNLU: https://github.com/IndoNLP/indonlu
- **Model IndoBERT dan framework IndoNLU** yang dikembangkan oleh **Wilie dkk. (2020)**. Kami sangat menghargai karya mereka yang sangat membantu penelitian NLP Bahasa Indonesia.

  > Wilie, B., Vincentio, K., Winata, G. I., Cahyawijaya, S., dkk. (2020). _IndoNLU: Benchmark and Resources for Evaluating Indonesian Natural Language Understanding_.  
  > Proceedings of AACL-IJCNLP 2020, hlm. 843–857.  
  > https://doi.org/10.18653/v1/2020.aacl-main.85

- **CNBC Indonesia** sebagai sumber teks judul berita yang digunakan dalam studi ini.  
  Kami mengucapkan terima kasih kepada CNBC Indonesia atas akses ke berita keuangan yang tersedia secara publik. Permohonan izin telah diajukan; namun, belum ada tanggapan. Karya ini dilakukan dalam kerangka fair use untuk penelitian akademik.

---

## 📚 Sitasi

Jika Anda menggunakan proyek atau dataset ini, mohon sitasi:
- https://doi.org/10.34740/kaggle/dsv/12604035 untuk dataset;
- https://doi.org/10.11591/ijeecs.v42.i3.pp774-785 untuk riset.

---

## ⚖️ Lisensi

Lisensi MIT – lihat file `LICENSE` untuk detailnya.

---

## 📬 Kontak

📧 tj.triagungj@gmail.com  
Silakan hubungi untuk pertanyaan, kolaborasi, atau masukan.