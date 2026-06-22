# 🛡️ Cybersecurity AI Copilot (GraphRAG System)

Aplikasi ini adalah **Agen AI Cybersecurity Cerdas** berbasis Graph Retrieval-Augmented Generation (GraphRAG). Sistem ini dirancang untuk membaca jutaan data ancaman siber (Phishing, Defacement, Malware) dan menggunakan kecerdasan buatan untuk memberikan rekomendasi keamanan secara *real-time*.

## 🚀 Fitur Utama (Tier 4 Capabilities)

1. **Text-to-Cypher / Graph Analytics:** AI tidak hanya mencari teks, tetapi dapat menulis kueri database (Cypher) secara mandiri untuk melakukan perhitungan agregasi matematis dari puluhan ribu data.
2. **LLM Graph Builder (Unstructured Data ETL):** Sistem mampu membaca teks berita mentah/artikel ancaman terbaru, mengekstrak entitasnya, dan secara otomatis menyusunnya menjadi relasi di dalam Graph Database.
3. **Smart Fallback Reasoning (Nalar AI):** Jika URL atau ancaman baru tidak ditemukan di dalam database historis, AI tidak akan *error*. Ia akan bertindak sebagai analis siber menggunakan wawasan umumnya untuk membedah struktur domain (TLD), mendeteksi potensi *typosquatting*, dan memberikan mitigasi darurat.

## 🛠️ Tech Stack
* **Database:** Neo4j (Graph Database)
* **LLM Engine:** Groq API (Llama-3.3-70b-versatile) untuk *inferencing* berkecepatan tinggi.
* **Orchestration:** LangChain & LangChain Graph
* **Data Processing:** Pandas & Python

## 📸 Dokumentasi & Hasil Pengujian

*(Ganti teks di bawah ini dengan gambar screenshot yang kamu ambil)*

### 1. Visualisasi Graph Database
> `![Screenshot Visualisasi Neo4j Sandbox](link-gambar-di-sini)`
> Visualisasi relasi antara Node URL, Domain, TLD, dan Label Klasifikasi Ancaman dari 30.000 data dataset.

### 2. Skenario Pengujian: Analisis TLD Paling Berbahaya (Agregasi Graf)
> `![Screenshot Test Agregasi](link-gambar-di-sini)`
> AI berhasil menghitung dan mengurutkan Top-Level Domain (TLD) yang paling banyak digunakan untuk *phishing* langsung dari database.

### 3. Skenario Pengujian: Smart Fallback (Deteksi Taktik Social Engineering)
> `![Screenshot Test Link Random](link-gambar-di-sini)`
> AI membedah tautan asing (`netflix-update-payment.xyz`) yang tidak ada di database dan berhasil mendeteksi manipulasi *typosquatting*.

---
**Dikembangkan untuk pemenuhan tugas implementasi sistem cerdas.**