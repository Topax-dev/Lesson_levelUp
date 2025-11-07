# 🧩 Latihan Prisma dan GitHub API

Proyek ini merupakan latihan integrasi **Prisma ORM** dengan **GitHub API (Raw Content)** menggunakan **Express.js**.  
Tujuannya adalah untuk mempelajari bagaimana cara mengambil file Markdown dari repository GitHub, lalu menyimpannya ke database menggunakan Prisma.

---

## 📚 Lesson contents
- [🚀 Fitur Utama](#fitur-utama)
- [🧠 Tujuan Pembelajaran](#-tujuan-pembelajaran)
- [⚙️ Teknologi yang Digunakan](#-teknologi-yang-digunakan)
- [🧩 Struktur Proyek](#-struktur-proyek)
- [📦 Instalasi dan Setup](#-instalasi-dan-setup)
- [🧪 Cara Penggunaan](#-cara-penggunaan)
- [📄 Lisensi](#-lisensi)

---

## 🚀 Fitur Utama

- Menampilkan daftar lesson dari database  
- Mengambil konten lesson dari GitHub  
- Menyimpan hasil fetch ke kolom `content`  
- Menambahkan waktu sinkronisasi (`lastSyncedAt`)  
- Menandai konten yang telah diubah (`isEdited`)

---

## 🧠 Tujuan Pembelajaran

1. Memahami penggunaan **Prisma ORM** untuk operasi CRUD  
2. Belajar cara melakukan **fetch data eksternal** menggunakan `fetch()`  
3. Mengerti bagaimana cara **update data otomatis** ke database  
4. Membiasakan diri dengan **struktur project Express.js**

---

## ⚙️ Teknologi yang Digunakan

- Node.js
- Express.js
- Prisma ORM
- Axios / Fetch API
- MySQL atau PostgreSQL
- JavaScript (ES Module)

---

## 🧩 Struktur Proyek
```bash
project-root/
│
├── prisma/
│   └── schema.prisma
│
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── services/
│   └── index.js
│
├── package.json
└── README.md
