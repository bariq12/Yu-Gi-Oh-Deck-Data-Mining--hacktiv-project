# Yu-Gi-Oh-Deck-Data-Mining--hacktiv-project  

##  Project Overview  
Project ini bertujuan untuk menganalisis data deck permainan **Yu-Gi-Oh!** menggunakan pendekatan **AI (Large Language Model via LangChain + Replicate API)** serta teknik analisis data.  

Fokus utama:  
- Mengklasifikasikan dan menganalisis komposisi kartu berdasarkan format deck (*Meta, Non-Meta, Fun, Tournament*).  
- Mengidentifikasi **20 kartu yang paling sering digunakan** dalam setiap format.  
- Menyajikan hasil analisis dalam bentuk **visualisasi grafik** agar mudah dipahami.  

---

##  Raw Dataset Link  
Dataset mentah: yugioh_deck.csv

Informasi dataset:  
- Jumlah data: **±1696 deck**  
- Kolom utama:  
  - `deck_name` → Nama deck  
  - `format` → Jenis format (Meta, Non-Meta, Fun, Tournament, dll.)  
  - `main_deck`, `extra_deck`, `side_deck` → List kartu dalam setiap deck  

---

## Masalah & Tujuan  
**Masalah:**  
- Banyaknya variasi deck dan kartu membuat pemain sulit memahami meta terkini.  
- Pemain kesulitan mengetahui kartu mana yang paling dominan dalam setiap format.  

**Tujuan:**  
1. Membuat analisis otomatis yang menampilkan **kartu paling populer** per format.  
2. Memberikan gambaran visual tentang **tren meta Yu-Gi-Oh!** secara cepat dan akurat.  
3. Menjadi referensi bagi pemain untuk **membangun deck lebih efektif** sesuai tren permainan.  

---

##  Insight & Findings  
Hasil analisis awal menunjukkan:  
- Ada kartu *staple* yang muncul di hampir semua kategori format.  
- Distribusi format menunjukkan dominasi **Non-Meta Decks** sebagai kategori terbesar dalam dataset.  
- Analisis grafik membantu membandingkan **popularitas kartu antar format** dengan jelas.  

---

##  AI Support Explanation  
Project ini didukung oleh **AI/LLM** untuk analisis data.  

- **Framework:** [LangChain](https://www.langchain.com/)  
- **Model LLM:** [Replicate API](https://replicate.com/) dengan model `ibm-granite/granite-3.3-8b-instruct`  
- **Peran AI dalam project:**  
  - Mengambil **Top-20 kartu per format** langsung dari dataset.  
  - Membuat **visualisasi bar chart** dengan instruksi natural language.  
  - Mendukung eksplorasi data interaktif melalui query teks sederhana.  

---

##  Output yang Dihasilkan  
- **Top 20 kartu paling sering digunakan** (per format dan keseluruhan).  
- **Grafik bar chart** yang menunjukkan perbandingan popularitas kartu.  
- **Distribusi format deck** dalam dataset.  
- **Insight meta Yu-Gi-Oh!** yang bisa menjadi panduan untuk pemain maupun peneliti data.  
