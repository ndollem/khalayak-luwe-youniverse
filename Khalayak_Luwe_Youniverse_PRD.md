# 🧾 Product Requirements Document (PRD)

## 📌 Project Name
**Khalayak Luwe Youniverse**

## 🗓️ Version
v1.0 — Static Web Launch

## 👥 Project Owner
Agus Salim & Friends

## 🎯 Purpose
Khalayak Luwe Youniverse adalah sebuah halaman web statis yang berfungsi sebagai **pusat akses QRIS dari beberapa lapak teman** (UMKM, warung, pedagang kaki lima, dll), sehingga siapapun dapat melakukan pembayaran digital lewat **satu halaman website ringan dan responsif.**

Tujuan utamanya adalah **mempermudah pembayaran tanpa perlu mencari QRIS satu per satu**, serta memberikan **eksposur dan identitas digital sederhana** untuk setiap lapak yang tergabung.

---

## 🧠 Product Overview

### 🏁 Goals
1. Menyediakan **halaman tunggal** yang menampilkan QRIS dari 5 lapak berbeda.
2. Memudahkan pengguna melakukan pembayaran digital melalui **scan QRIS langsung dari browser** (menggunakan kamera atau Google Lens).
3. Membuat tampilan **modern, ringan, dan mudah diakses di perangkat mobile.**
4. Dapat dihosting **gratis dan cepat di GitHub Pages.**

### 📱 Target Users
- Pelanggan yang ingin membayar produk dari salah satu lapak.
- Pemilik lapak yang ingin membagikan halaman pembayaran kepada pembeli.
- Pengunjung umum yang ingin mendukung UMKM lokal.

---

## ⚙️ Functional Requirements

| Fitur | Deskripsi | Prioritas |
|-------|------------|------------|
| **Daftar Lapak (5 item)** | Menampilkan 5 lapak berbeda dalam bentuk grid responsif. | ⭐⭐⭐⭐⭐ |
| **Informasi Lapak** | Tiap lapak memiliki: nama, nama pemilik, deskripsi singkat produk, dan gambar QRIS. | ⭐⭐⭐⭐⭐ |
| **Desain Responsif** | Layout otomatis menyesuaikan untuk mobile dan desktop. | ⭐⭐⭐⭐ |
| **Warna Unik per Lapak** | Tiap card lapak punya warna/aksen berbeda untuk mudah dibedakan. | ⭐⭐⭐ |
| **Petunjuk Scan QRIS** | Teks atau ikon yang menjelaskan cara scan menggunakan Google Lens. | ⭐⭐⭐⭐⭐ |
| **Hosting di GitHub Pages** | Website dapat diakses publik secara gratis. | ⭐⭐⭐⭐ |
| **Optimasi Gambar** | Ukuran QRIS tidak besar agar halaman tetap cepat dimuat. | ⭐⭐⭐⭐ |

---

## 🎨 Design Requirements

### Layout
- Struktur utama:
  ```
  Header
  ↓
  Grid Card Lapak (5)
  ↓
  Footer (Petunjuk scan)
  ```
- Menggunakan **Tailwind CSS CDN** untuk styling.
- Grid responsif:  
  - Mobile → 1 kolom  
  - Desktop → 2 kolom

### Style Guide
| Elemen | Gaya |
|--------|------|
| Font | Sans-serif (Poppins / Inter) |
| Warna dasar | `bg-gray-50`, teks `text-gray-800` |
| Card | `rounded-xl`, `shadow-md`, `hover:shadow-lg`, `transition-all` |
| Warna Card Lapak | Gunakan kombinasi lembut: biru muda, hijau muda, merah muda, ungu muda, kuning muda |
| QRIS Image | `max-w-xs mx-auto rounded-lg border` |
| Interaksi | Hover scale + shadow untuk efek responsif visual |

---

## 🧩 Content Structure

| Field | Contoh |
|--------|--------|
| Nama Lapak | Warung Mie Enak |
| Pemilik | Bu Siti |
| Deskripsi | Menjual Mie Goreng, Mie Rebus, dan Telur Dadar |
| Gambar QRIS | `/img/mie-enak-qris.png` |
| Warna Card | `bg-blue-100` |

---

## 🚀 Technical Requirements

| Komponen | Detail |
|-----------|---------|
| Framework | HTML + Tailwind CSS (CDN) |
| Hosting | GitHub Pages |
| Responsivitas | Flex/Grid layout |
| File Struktur |  
```
/index.html  
/img/ (folder QRIS images)  
/README.md (opsional)
``` |
| Browser Support | Chrome, Safari, Firefox, Edge (mobile dan desktop) |

---

## 🧭 User Flow

1. Pengunjung membuka halaman `https://username.github.io/khalayak-luwe-youniverse`
2. Melihat daftar 5 lapak dalam tampilan grid.
3. Memilih lapak tujuan berdasarkan nama/deskripsi.
4. Melihat gambar QRIS dan instruksi scan.
5. Menggunakan Google Lens / kamera untuk melakukan pembayaran.
6. (Opsional) Kembali dan memilih lapak lain.

---

## 🧰 Non-Functional Requirements

| Aspek | Deskripsi |
|-------|------------|
| Performance | Halaman < 1MB total (loading < 2 detik di mobile). |
| Accessibility | Teks kontras tinggi, gambar dengan alt text. |
| Maintainability | Mudah menambah lapak baru dengan menyalin satu blok `<div>` card. |
| SEO | Title dan meta description berisi kata kunci “QRIS UMKM / Pembayaran digital”. |

---

## 📅 Milestone Plan

| Tahap | Kegiatan | Estimasi Waktu |
|--------|-----------|----------------|
| 1 | Rancang layout & PRD | 1 hari |
| 2 | Buat struktur HTML + Tailwind | 1 hari |
| 3 | Tambah data & gambar QRIS | 1 hari |
| 4 | Testing mobile & desktop | 0.5 hari |
| 5 | Deploy ke GitHub Pages | 0.5 hari |

**Total:** ± 3 hari kerja ringan.

---

## 🔮 Future Enhancements (Opsional)

| Ide | Deskripsi |
|-----|------------|
| Filter / Search | Memungkinkan user mencari lapak berdasarkan nama/jenis jualan. |
| QRIS Popup Modal | QRIS muncul dalam modal agar tampak lebih besar di layar kecil. |
| Analytics | Tracking jumlah pengunjung tiap lapak. |
| Dark Mode | Menyesuaikan tampilan sesuai preferensi pengguna. |

---

## 🏁 Deliverable
1. File `index.html` siap upload ke GitHub Pages.  
2. Folder `img/` berisi QRIS tiap lapak.  
3. README.md (opsional) menjelaskan proyek dan cara kontribusi.
