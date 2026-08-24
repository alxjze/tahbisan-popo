# PT. Laksamana Container International — Landing Page

Satu berkas `index.html` tanpa dependensi dan tanpa proses build. Desain dan palet
warna halaman mengikuti identitas grup Laksamana (biru korporat `#1B3FA5`, merah aksen
`#EF3E33`, putih), agar sejalan dengan situs
[PT. Laksamana Chaidir Indonesia](https://www.laksamanachaidirindonesia.com/).
Lambang perusahaan digambar sebagai SVG sebaris — tiga lapisan bertumpuk
(kuning `#E9A825`, hijau `#4CAF50`, biru `#2C82C9` dengan mata panah).

## Bagian halaman

Beranda (hero + statistik) · Pita grup · Tentang Kami (visi & misi) · Layanan (9 kartu) ·
Jenis Kontainer (6 tipe) · Keunggulan · Alur Kerja · Sektor yang Dilayani · FAQ ·
Kontak (formulir → WhatsApp) · CTA · Footer.

## Yang perlu diganti sebelum tayang

Nomor WhatsApp resmi sudah terpasang: **+62 812-8579-4886** (`6281285794886`, dipakai di
konstanta `WA_NUMBER`, tautan `wa.me`, footer, dan JSON-LD). Sisanya masih sementara dan
ditandai komentar `<!-- TODO -->` di dalam berkas:

| Isi | Nilai sementara |
| --- | --- |
| Surel | `info@laksamanacontainer.co.id` |
| Alamat kantor & depo | "Kawasan Pelabuhan Tanjung Priok, Jakarta Utara 14310" |
| Peta lokasi | kotak kosong — ganti dengan `<iframe>` Google Maps |
| Angka statistik hero | 15.000+ TEUs · 150+ armada · 10 menit ke terminal |
| Data JSON-LD di bagian bawah berkas | mengikuti nilai sementara di atas |

Angka statistik, kapasitas, dan jam operasional adalah contoh untuk keperluan
tata letak. Sesuaikan dengan data resmi perusahaan sebelum dipublikasikan.

## Menjalankan secara lokal

```bash
python3 -m http.server 8000
```

Lalu buka `http://localhost:8000/laksamana-container/`.
