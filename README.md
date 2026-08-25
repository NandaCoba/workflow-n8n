# Workflow n8n

Kumpulan workflow n8n untuk mengirim alert lowongan kerja teknologi ke Telegram dari beberapa sumber publik.

## Isi Repository

| File | Deskripsi |
| --- | --- |
| `telegram_junior_tech_jobs_n8n.json` | Workflow alert lowongan junior tech dari berbagai sumber, tanpa AI. |
| `telegram_multi_source_backend_job_alert_n8n.json` | Workflow alert lowongan backend dari berbagai sumber, tanpa AI. |
| `telegram_multi_source_varied_jobs_n8n.json` | Workflow alert lowongan tech yang lebih bervariasi dari berbagai sumber, tanpa AI. |

## Fitur

- Menarik data lowongan dari Remotive, RemoteOK, Arbeitnow, WeWorkRemotely, LinkedIn, Jobicy, dan Himalayas sesuai workflow.
- Normalisasi data dari beberapa format sumber.
- Filter dan deduplikasi lintas sumber.
- Skip lowongan yang sudah pernah dikirim.
- Format pesan otomatis untuk Telegram.
- Bisa dijalankan manual atau terjadwal setiap 3 jam.

## Cara Menggunakan

1. Buka n8n.
2. Pilih **Import from File**.
3. Pilih salah satu file workflow `.json` dari repository ini.
4. Buka node `CONFIG - EDIT ME`.
5. Isi konfigurasi yang diperlukan, terutama token bot Telegram dan chat ID.
6. Jalankan workflow secara manual untuk tes.
7. Aktifkan workflow jika hasil tes sudah sesuai.

## Catatan Konfigurasi

- Pastikan credential atau token Telegram tidak disimpan langsung ke repository publik.
- Beberapa sumber publik dapat mengubah format data atau membatasi request sewaktu-waktu.
- Sesuaikan keyword, lokasi, dan filter di node konfigurasi atau node kode jika diperlukan.

## Lisensi

Proyek ini menggunakan lisensi MIT. Lihat [LICENSE](LICENSE) untuk detail.
