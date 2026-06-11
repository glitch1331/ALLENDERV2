# ALLENDERV2
ALLENDER CALENDAR & ALARM SYSTEM
Live: https://allenderv-2.vercel.app/ 
FITUR:
-CALENDAR: Tampilkan, tambah, dan hapus event Google Calendar secara real-time
-ALARM: Alarm berulang (per hari) atau sekali di tanggal tertentu dengan interval & ringtone custom
-COUNTDOWN: Hitung mundur ke tanggal & waktu target
-IMPORT CSV: Import event secara jumlah besar ke Google Calendar dari file CSV atau paste teks dengan format CSV
-DARK MODE: Toggle Dark/Light mode
-DESKTOP AND MOBILE COMPATIBLE

Cara Pakai:
Fitur Calendar dan Import memerlukan akun Google. Klik Sign in with Google di halaman Calendar. (Email harus terdaftar di Google Cloud Console)
Alarm dan Countdown bisa dipakai tanpa login.

Set Alarm:
1. Buka tab Alarms → klik + New Alarm
2. Pilih waktu dan label
3. Pilih tipe:
  -Hari Berulang — alarm berbunyi setiap hari yang dipilih (Su/Mo/Tu/We/Th/Fr/Sa)
  -Tanggal Spesifik — alarm berbunyi sekali pada tanggal & waktu tertentu
4.Opsional: tambah interval untuk set beberapa alarm sekaligus dari satu waktu base
5. Pilih ringtone → klik Set Alarm

Countdown:
1. Buka tab Countdown
2. Isi tanggal target, waktu target, dan nama event
3. Pilih ringtone yang akan berbunyi saat selesai
4. Klik ▶ Mulai

Import CSV:
1. Buka tab Import
2. Drop file CSV, klik browse, atau paste teks langsung
3. Preview event yang terdeteksi
4. Klik Import ke Google Calendar
Format:
title, start, end, note
Rapat Tim, 2026-06-15T09:00, 2026-06-15T10:00, Weekly
Ujian, 2026-06-20T08:00, 2026-06-20T12:00,
Note: start / end dalam format ISO 8601: YYYY-MM-DDTHH:MM

Teknologi:
HTML + CSS + Vanilla JS: tidak ada framework
Google Calendar API v3:untuk baca/tulis event
Google Identity Services: OAuth 2.0 login
Web Audio API: ringtone built-in (Beep, Chime, Buzz, Retro)
HTML5 Audio: untuk ringtone custom yang diupload user
Vercel: hosting web static

Struktur:
allender berisi 2 file yaitu
- index.html (HTML, CSS dan javascript
- vercel.json  (konfigurasi deploy dari Vercel)

Notes:
- Data alarm tidak tersimpan jika halaman di-refresh (tersimpan di memori saja)
- Alarm hanya berbunyi selama tab browser aktif
- Saat status OAuth masih Testing, hanya email yang terdaftar sebagai test user yang bisa login — tambahkan email di Google Cloud Console → Audience → Test Users
