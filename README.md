# Website Joki Tugas (Static)

Website landing page joki tugas dengan layout modern (Bootstrap 5) dan 2 integrasi API publik menggunakan fetch dari browser:

- API 1: GitHub Users → menampilkan kartu tim (avatar + link profil)
- API 2: JSONPlaceholder Posts → menampilkan kartu tips/blog

## Cara Menjalankan

Karena proyek ini bersifat static, cukup buka file `index.html` langsung di browser:

- Windows: klik dua kali `index.html` atau klik kanan → Open With → pilih browser
- Atau jalankan server static (opsional) jika ingin menghindari kendala CORS tertentu:

```bash
python -m http.server 8000
```

Lalu buka `http://localhost:8000`.

## Fitur

- Layout responsif dengan Bootstrap 5 + Bootstrap Icons via CDN
- Navigasi ke bagian: Beranda, Layanan, Tim (API GitHub), Tips (API JSONPlaceholder), Pemesanan
- Form pemesanan dengan validasi client-side dan pesan sukses
- Kartu layanan dengan harga, CTA, dan efek hover
- Seksi tim dan tips terisi dinamis dari API pihak ketiga

## Struktur File

- `index.html` — seluruh halaman (multi-section) dan script integrasi API
- `README.md` — petunjuk penggunaan

## Catatan

- Jika koneksi ke API publik diblokir jaringan, bagian Tim/Tips akan menampilkan pesan peringatan.
- Tidak ada backend: form hanya menampilkan notifikasi sukses. Integrasi WhatsApp/Email dapat ditambahkan sesuai kebutuhan.
