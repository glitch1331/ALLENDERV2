# ALLENDER
ALLENDER CALENDAR & ALARM SYSTEM
Live: https://allenderv-2.vercel.app/ 

ALLENDER adalah aplikasi berbasis web yang mengintegrasikan kalender, alarm, dan countdown timer dalam satu platform. Aplikasi ini dirancang untuk membantu pengguna mengelola jadwal, alarm, serta tenggat waktu dengan lebih efisien melalui antarmuka yang sederhana, modern, dan responsif.

LATAR BELAKANG:
Dalam kehidupan sehari-hari, pengguna sering menggunakan beberapa aplikasi berbeda untuk mengelola aktivitas mereka, seperti:
- Aplikasi kalender untuk mencatat jadwal.
- Aplikasi alarm untuk pengingat.
- Aplikasi countdown untuk menghitung mundur menuju suatu acara.
- Spreadsheet untuk mengelola data jadwal dalam jumlah besar.

Penggunaan banyak aplikasi secara terpisah menyebabkan beberapa kendala, antara lain:
- Informasi jadwal tersebar di berbagai platform.
- Pengguna harus memasukkan data yang sama berulang kali.
- Sulit memantau tenggat waktu dan pengingat dalam satu tampilan.
- Tidak tersedia fitur impor data jadwal secara jumlah besar.

SOLUSI:
ALLENDER hadir sebagai solusi dengan menggabungkan fungsi kalender, alarm, countdown timer, dan impor data dalam satu aplikasi terintegrasi.
Melalui integrasi dengan Google Calendar, pengguna dapat mengelola seluruh aktivitas dan pengingat tanpa perlu berpindah-pindah aplikasi.

MANFAAT:
- Mengelola jadwal dan pengingat dalam satu aplikasi.
- Mengurangi penggunaan banyak aplikasi secara bersamaan.
- Memantau deadline dan acara penting dengan lebih mudah.
- Mengimpor jadwal dalam jumlah besar secara cepat.
- Meningkatkan produktivitas dalam mengatur aktivitas sehari-hari.

FITUR:

-CALENDAR:
  - Menampilkan jadwal dalam tampilan kalender bulanan.
  - Menambahkan event baru.
  - Menghapus event.
  - Sinkronisasi langsung dengan akun Google Calendar.

-ALARM:
  - Membuat alarm satu kali.
  - Membuat alarm berulang (Recurring Alarm).
  - Memberikan label pada alarm.
  - Menentukan interval pengingat.
  - Menggunakan ringtone custom.
  - Menampilkan notifikasi alarm secara visual.

-COUNTDOWN:
  - Menghitung mundur menuju tanggal dan waktu tertentu.
  - Memberikan nama pada countdown.
  - Menampilkan sisa waktu secara real-time.
  - Memutar notifikasi ketika countdown selesai.

-IMPORT CSV:
  - Import jadwal dari file CSV.
  - Drag & drop file CSV.
  - Paste data CSV langsung ke web.
  - Menambahkan event ke Google Calendar secara jumlah besar.

-SIMPLE AND MODERN DESIGN:
  - Dark and Light Mode
  - Tampilan sederhana dan mudah digunakan.
  - Responsive untuk desktop dan mobile

Cara Pakai:
Fitur Calendar dan Import memerlukan akun Google. Klik Sign in with Google di halaman Calendar. (Email harus terdaftar di Google Cloud Console)
Alarm dan Countdown bisa dipakai tanpa login.

Set Alarm:
1. Buka tab Alarms → klik + New Alarm
2. Pilih waktu dan label
3. Pilih tipe:
  -Hari Berulang (alarm berbunyi setiap hari yang dipilih)
  -Tanggal Spesifik (alarm berbunyi sekali pada tanggal & waktu tertentu)
4.Tambah interval untuk set beberapa alarm sekaligus (opsional)
Contoh:
  - Base: 07:00
  - +15 menit → alarm ke-2 jam 07:15
  - +30 menit → alarm ke-3 jam 07:30
5. Pilih ringtone → klik Set Alarm

Countdown:
1. Buka tab Countdown
2. Isi tanggal target, waktu target, dan nama event
3. Pilih ringtone yang akan berbunyi saat selesai
4. Klik Mulai

Import CSV:
1. Buka tab Import
2. Drop file CSV, klik browse, atau paste teks langsung
3. Preview event yang terdeteksi
4. Klik Import ke Google Calendar
Format:
title, start, end, note
Rapat Tim, 2026-06-15T09:00, 2026-06-15T10:00, Weekly
Ujian, 2026-06-20T08:00, 2026-06-20T12:00,

Teknologi:
HTML + CSS + Vanilla JS
Google Calendar API: untuk baca/tulis event
Google Identity Services: OAuth login
Web Audio API: ringtone built-in (Beep, Chime, Buzz, Retro)
HTML5 Audio: untuk ringtone custom yang diupload user
Vercel: hosting web static

Struktur:
allender berisi 2 file yaitu
- index.html (HTML, CSS dan vanilla JavaScript)
- vercel.json  (konfigurasi deploy dari Vercel)

Notes:
- Data alarm tidak tersimpan jika halaman di-refresh (tersimpan di memori saja)
- Alarm hanya berbunyi selama tab browser aktif
- Note: start / end dalam format ISO 8601: YYYY-MM-DDTHH:MM
