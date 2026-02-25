# Cloud-Computing-KickOff-Project
Project Cloud Computing Praktikum Kelompok sebelum UTS, semester 6 program studi D4 Teknik Informatika

## Deskripsi
Project ini merupakan sistem presensi berbasis web menggunakan QR Code.  
Mahasiswa melakukan presensi dengan memindai QR Code, kemudian data dikirim ke backend untuk divalidasi dan disimpan.

## Tech Stack
- Google Apps Script (Backend)
- GitHub Pages (Frontend)
- Google Spreadsheet (Database)
- Postman (API Testing)

## Fitur Utama
- Presensi menggunakan QR Code
- Validasi token QR
- Penyimpanan data presensi
- Monitoring status presensi

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

## Cara Testing
1. Akses halaman deployment
2. Lakukan scan QR Code
3. Data dikirim ke backend
4. Response ditampilkan ke user
5. Testing API dapat dilakukan menggunakan Postman

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
