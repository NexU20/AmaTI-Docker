# 📦 Project Setup Guide

Panduan ini menjelaskan langkah-langkah untuk menjalankan proyek menggunakan **Docker Compose** dan **Prisma**.

---

## 🚀 Prasyarat

Pastikan Anda sudah menginstal:
- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

---

## 🔧 Langkah-Langkah Instalasi

### 1. Jalankan Docker Compose

Buka terminal dan jalankan perintah berikut untuk memulai semua container:

```bash
docker compose up
```

Perintah ini akan membangun dan menjalankan container untuk aplikasi.

---

### 2. Migrasi Prisma

Setelah semua container berjalan, buka terminal baru dan jalankan perintah berikut untuk melakukan migrasi database:

```bash
docker exec amati_app npm run prisma-migrate
```

---

### 3. Inisialisasi Aplikasi

Setelah migrasi selesai, jalankan perintah berikut untuk menginisialisasi aplikasi:

```bash
docker exec amati_app npm run init
```

---

### 4. Selesai 🎉

Aplikasi Anda sudah berjalan dan siap digunakan!
