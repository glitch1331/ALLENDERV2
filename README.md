<p align="center">
  <img width="180" src="https://cdn-icons-png.flaticon.com/512/747/747310.png">
</p>

<p align="center">
  Smart Calendar • Alarm • Countdown Management System
</p>

<p align="center">
  🌐 https://allenderv-2.vercel.app/
</p>

---

# 📅 ALLENDER

ALLENDER adalah aplikasi berbasis web yang mengintegrasikan **Kalender**, **Alarm**, dan **Countdown Timer** dalam satu platform. Aplikasi ini dirancang untuk membantu pengguna mengelola jadwal, alarm, serta tenggat waktu dengan lebih efisien melalui antarmuka yang sederhana, modern, dan responsif.

---

## 📌 Overview

| Informasi     | Detail                                 |
| ------------- | -------------------------------------- |
| Nama Aplikasi | ALLENDER                               |
| Tipe          | Calendar & Alarm System                |
| Platform      | Web Application                        |
| URL           | https://allenderv-2.vercel.app/        |
| Fokus         | Manajemen Jadwal, Alarm, dan Countdown |
| Integrasi     | Google Calendar                        |
| Hosting       | Vercel                                 |

---

## 🚨 Latar Belakang

Dalam kehidupan sehari-hari, pengguna sering menggunakan beberapa aplikasi berbeda untuk mengelola aktivitas mereka, seperti:

* 📅 Aplikasi kalender untuk mencatat jadwal.
* ⏰ Aplikasi alarm untuk pengingat.
* ⌛ Aplikasi countdown untuk menghitung mundur menuju suatu acara.
* 📊 Spreadsheet untuk mengelola data jadwal dalam jumlah besar.

Penggunaan banyak aplikasi secara terpisah menyebabkan beberapa kendala, antara lain:

* ❌ Informasi jadwal tersebar di berbagai platform.
* ❌ Pengguna harus memasukkan data yang sama berulang kali.
* ❌ Sulit memantau tenggat waktu dan pengingat dalam satu tampilan.
* ❌ Tidak tersedia fitur impor data jadwal dalam jumlah besar.

---

## 💡 Solusi

ALLENDER hadir sebagai solusi dengan menggabungkan fungsi kalender, alarm, countdown timer, dan impor data dalam satu aplikasi terintegrasi.

Melalui integrasi dengan Google Calendar, pengguna dapat mengelola seluruh aktivitas dan pengingat tanpa perlu berpindah-pindah aplikasi.

```text
            ┌─────────────┐
            │   Calendar  │
            └──────┬──────┘
                   │
                   ▼
        ┌─────────────────────┐
        │      ALLENDER       │
        └─────────────────────┘
          │       │        │
          ▼       ▼        ▼
       Alarm  Countdown  CSV Import
```

---

## 🎯 Manfaat

Dengan menggunakan ALLENDER, pengguna dapat:

✅ Mengelola jadwal dan pengingat dalam satu aplikasi.

✅ Mengurangi penggunaan banyak aplikasi secara bersamaan.

✅ Memantau deadline dan acara penting dengan lebih mudah.

✅ Mengimpor jadwal dalam jumlah besar secara cepat.

✅ Meningkatkan produktivitas dalam mengatur aktivitas sehari-hari.

---

# ✨ Fitur Utama

## 📅 Calendar

* Menampilkan jadwal dalam tampilan kalender bulanan.
* Menambahkan event baru.
* Menghapus event.
* Sinkronisasi langsung dengan akun Google Calendar.

---

## ⏰ Alarm

* Membuat alarm satu kali.
* Membuat alarm berulang (*Recurring Alarm*).
* Memberikan label pada alarm.
* Menentukan interval alarm.
* Menggunakan ringtone custom.
* Menampilkan notifikasi alarm secara visual.

---

## ⌛ Countdown

* Menghitung mundur menuju tanggal dan waktu tertentu.
* Memberikan nama pada countdown.
* Menampilkan sisa waktu secara real-time.
* Memutar notifikasi ketika countdown selesai.

---

## 📂 Import CSV

* Import jadwal dari file CSV.
* Drag & Drop file CSV.
* Paste data CSV langsung ke web.
* Menambahkan event ke Google Calendar secara jumlah besar.

---

## 🎨 Simple & Modern Design

* 🌙 Dark Mode
* ☀️ Light Mode
* 📱 Responsive untuk desktop dan mobile
* ✨ Tampilan sederhana dan mudah digunakan

---

# 🚀 Cara Pakai

## Login Google

Fitur **Calendar** dan **Import CSV** memerlukan akun Google.

Klik **Sign in with Google** pada halaman Calendar untuk mulai menggunakan fitur sinkronisasi Google Calendar.

> Alarm dan Countdown dapat digunakan tanpa login.

---

## ⏰ Membuat Alarm

1. Buka tab **Alarms**.
2. Klik **+ New Alarm**.
3. Pilih waktu dan label alarm.
4. Pilih tipe alarm:

   * **Hari Berulang** → alarm berbunyi setiap hari yang dipilih.
   * **Tanggal Spesifik** → alarm berbunyi sekali pada tanggal dan waktu tertentu.
5. Tambahkan interval untuk membuat beberapa alarm sekaligus (opsional).

Contoh:

```text
Base Alarm : 07:00
+15 Menit  : 07:15
+30 Menit  : 07:30
```

6. Pilih ringtone.
7. Klik **Set Alarm**.

---

## ⌛ Membuat Countdown

1. Buka tab **Countdown**.
2. Isi tanggal target.
3. Isi waktu target.
4. Masukkan nama event.
5. Pilih ringtone.
6. Klik **Mulai**.

---

## 📂 Import CSV

1. Buka tab **Import**.
2. Drop file CSV, klik browse, atau paste data CSV langsung.
3. Preview event yang terdeteksi.
4. Klik **Import ke Google Calendar**.

### Format CSV

```csv
title,start,end,note
Rapat Tim,2026-06-15T09:00,2026-06-15T10:00,Weekly
Ujian,2026-06-20T08:00,2026-06-20T12:00,
```

---

# ⚙️ Teknologi yang Digunakan

## Frontend

* HTML
* CSS
* Vanilla JavaScript

## API & Services

* Google Calendar API → baca/tulis event kalender.
* Google Identity Services → OAuth Login.

## Audio

* Web Audio API → ringtone bawaan (Beep, Chime, Buzz, Retro).
* HTML5 Audio → ringtone custom yang diunggah pengguna.

## Deployment

* Vercel → Hosting Web Static.

---

# 📁 Struktur Proyek

```text
ALLENDER/
│
├── index.html
└── vercel.json
```

### Keterangan

* `index.html` → HTML, CSS, dan seluruh Vanilla JavaScript aplikasi.
* `vercel.json` → konfigurasi deployment Vercel.

---

# 📝 Notes

* Data alarm tidak tersimpan jika halaman di-refresh (hanya tersimpan di memori browser).
* Alarm hanya dapat berbunyi selama tab browser masih aktif.
* Format tanggal menggunakan standar ISO 8601:

```text
YYYY-MM-DDTHH:MM
```

Contoh:

```text
2026-06-15T09:00
```

---

# 🌐 Live Demo

https://allenderv-2.vercel.app/

---

## 👨‍💻 Developer

Developed with ❤️ using HTML, CSS, Vanilla JavaScript, Google Calendar API, and Vercel.
