# WaeGuide AI: Smart Cultural Assistant for Rural Tourism

**WaeGuide AI** adalah solusi asisten virtual berbasis suara yang dirancang khusus untuk wisatawan di Desa Wisata Wae Rebo. Fokus utama proyek ini adalah menyediakan akses informasi budaya yang mendalam dan manajemen layanan secara **offline**, mengingat keterbatasan akses internet di lokasi tujuan.

## 🚀 Fitur Utama

-   **Voice-Based Cultural Assistant**: Interaksi berbasis suara untuk menanyakan filosofi, sejarah, dan aturan adat (mirip Google Assistant).
-   **Offline Knowledge Engine**: Pemrosesan bahasa alami (NLP) dilakukan secara lokal di perangkat (*on-device*) tanpa membutuhkan koneksi internet.
-   **Contextual Audio Guide**: Memutar penjelasan audio yang relevan sesuai dengan konteks ritual adat yang sedang disaksikan.
-   **Unified Booking System**: Transparansi harga untuk layanan transportasi (ojek), akomodasi, dan konsumsi.
-   **Quick Translate Tool**: Alat bantu terjemahan sederhana untuk komunikasi teknis antara turis dan warga lokal.

## 🛠️ Tech Stack

-   **Mobile Framework**: Flutter (Cross-platform Android/iOS)
-   **Natural Language Processing (NLP)**: TensorFlow Lite (untuk *Intent Classification* luring)
-   **Database**: SQLite / Hive (Penyimpanan aset teks dan audio secara lokal)
-   **Speech-to-Text (STT) & TTS**: On-device Speech Recognition API

## 📂 Struktur Proyek (WIP)

```text
├── assets/             # Database audio (.mp3) dan metadata (.json)
├── docs/               # Proposal, Roadmap, dan UI/UX Screenshots
├── lib/                
│   ├── logic/          # Implementasi NLP & Offline Processing
│   ├── models/         # Struktur data (Culture, Price, User)
│   └── ui/             # Antarmuka aplikasi (Flutter)
└── README.md           # Dokumentasi utama
```

## 🧠 Cara Kerja "Offline Knowledge Engine"

1.  **Sync**: Pengguna mengunduh *knowledge pack* Wae Rebo saat masih ada sinyal.
2.  **Process**: Saat offline, suara pengguna diproses oleh **TensorFlow Lite** untuk menentukan *intent* (maksud pertanyaan).
3.  **Retrieve**: Aplikasi mengambil jawaban atau file audio yang sesuai dari database **SQLite** internal.
4.  **Output**: Jawaban disampaikan melalui teks atau suara secara instan tanpa *latency* internet.

---

### 🔑 Kredensial Demo (Prototype)
*   **Username**: `guest.waerebo@wguide.id`
*   **Password**: `WaeRebo2026`

---

**Catatan:** Proyek ini dikembangkan sebagai bagian dari **Dicoding Challenge**. Status saat ini adalah *Initial Prototype* dengan fokus pada validasi arsitektur sistem *Offline-First*.

---
