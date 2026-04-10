# 🛡️ HZT Guardian Monitor V1.0

**HZT Guardian Monitor** adalah alat monitoring server real-time berperforma tinggi yang dirancang khusus untuk server file berbasis Windows. Aplikasi ini menyediakan antarmuka widget modern yang elegan untuk memantau kesehatan sistem sekaligus menjaga keamanan data melalui sistem pertahanan aktif.

## 🚀 Fitur Utama

- **Metrik Sistem Live:** Pemantauan penggunaan CPU, RAM, dan GPU dengan animasi yang halus.
- **Visualisasi Multi-Storage:** Deteksi otomatis dan pemantauan kesehatan (Pie Chart) untuk semua SSD dan HDD yang terhubung.
- **Pelacak Trafik Jaringan:** Pemantauan kecepatan upload dan download secara real-time.
- **Keamanan Pertahanan Aktif (Tingkat Dewa):**
    - **Whitelist MAC Address:** Hanya perangkat resmi yang dapat mengakses direktori terlindungi.
    - **Sistem Auto-Sever:** Memutuskan sesi SMB yang tidak sah secara otomatis jika mencoba mengakses folder sensitif.
    - **Path Terlindungi:** Perlindungan folder kustom untuk data gaji, database, dan file internal.
- **UI/UX Modern:**
    - Desain sudut melengkung tanpa frame.
    - Mode widget yang bisa digeser dan "Always on Top".
    - Log keamanan informatif dengan kode warna.

## 🛠️ Teknologi yang Digunakan

- **Bahasa:** Python 3.14
- **Framework:** PySide6 (Qt for Python)
- **Library:** psutil, GPUtil

## 📥 Cara Instalasi

1. Buka halaman [Releases](https://github.com/hizpro/HZT-Guardian-Monitor/releases).
2. Download file `hzt_guardian.exe`.
3. Jalankan aplikasi sebagai **Administrator** (Wajib untuk fitur manajemen jaringan).

## 🔒 Konfigurasi Keamanan

Saat dijalankan pertama kali, aplikasi akan membuat file `whitelist.json`. Tambahkan MAC Address yang diizinkan ke dalam file ini untuk memberikan akses ke zona terlindungi.

```json
{
  "approved": ["00:15:5D:01:20:AF", "AA:BB:CC:DD:EE:FF"]
}
