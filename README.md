# Cloud-Computing-KickOff-Project
Project Cloud Computing Praktikum Kelompok sebelum UTS, semester 6 program studi D4 Teknik Informatika

## Deskripsi
Project ini merupakan sistem presensi berbasis web menggunakan QR Code.  
Mahasiswa melakukan presensi dengan memindai QR Code, kemudian data dikirim ke backend untuk divalidasi dan disimpan.

Selain fitur presensi, sistem ini juga mendukung pengiriman data sensor dari perangkat seperti **accelerometer** dan **GPS** untuk keperluan monitoring perangkat.

## Arsitektur Sistem

User Device (Browser / Mobile)  
↓  
Frontend (GitHub Pages)  
↓  
HTTP Request  
↓  
Backend API (Google Apps Script)  
↓  
Database (Google Spreadsheet)

## Tech Stack
- Google Apps Script (Backend)
- GitHub Pages (Frontend)
- Google Spreadsheet (Database)
- Postman (API Testing)
- Swagger (API Documentation)

## Fitur Utama
- Presensi menggunakan QR Code
- Validasi token QR
- Penyimpanan data presensi
- Monitoring status presensi
- Pengiriman data accelerometer
- Pengiriman dan penyimpanan data GPS
- Monitoring data sensor perangkat

## Base URL
https://script.google.com/macros/s/AKfycbxySS5-lojND4iGPC8mXwi9EDs01mbL50ncC4hT7sfkDZWQC-k3HNuDBtIQmyM7h965/exec

## Deployment
https://kamilasaadah.github.io/Cloud-Computing-KickOff-Project/

## Endpoint Summary

| Method | Endpoint | Deskripsi |
|------|--------|----------|
| POST | /scan-presence | Mencatat presensi berdasarkan QR |
| GET | /presence-status | Mengecek status presensi |
| POST | /generate-qr | Generate QR Code presensi |
| POST | /telemetry/accel | Mengirim data accelerometer dari perangkat |
| GET | /telemetry/accel/latest | Mengambil data accelerometer terbaru |
| POST | /telemetry/gps | Mengirim data lokasi GPS |
| GET | /telemetry/gps/latest | Mengambil lokasi GPS terbaru |
| GET | /telemetry/gps/history | Mengambil riwayat lokasi GPS |

## Cara Testing
1. Akses halaman deployment.
2. Lakukan scan QR Code untuk presensi.
3. Data akan dikirim ke backend dan disimpan ke database.
4. Response sistem ditampilkan kepada user.
5. API juga dapat diuji menggunakan **Postman**.

Untuk pengujian sensor:
- Kirim data **accelerometer** menggunakan endpoint `/telemetry/accel`
- Kirim data **GPS** menggunakan endpoint `/telemetry/gps`

## Dokumentasi
https://docs.google.com/document/d/15qucBpNdQBquqEQstzvqbC8hPQoBRXf2Ds04OsVF5Wo/edit

## Swagger Documentation
File dokumentasi API tersedia di `swagger.yaml`
dan dapat dibuka menggunakan https://editor.swagger.io/

## Pembagian Tugas
- Backend: Mila  
- Frontend: Wafi  
- QA & Testing: Festi  
- Dokumentasi & Deploy: Arum