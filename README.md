# 🏪 Khalayak Luwe Youniverse

Pusat pembayaran digital QRIS untuk UMKM sahabat. Bayar mudah, dukung usaha lokal! 💙

## 🎯 Tentang Proyek

**Khalayak Luwe Youniverse** adalah halaman web statis yang berfungsi sebagai pusat akses QRIS dari beberapa lapak teman (UMKM, warung, pedagang kaki lima). Website ini memudahkan pembayaran digital melalui satu halaman yang ringan dan responsif.

## ✨ Fitur Utama

- 📱 **5 Lapak UMKM** dengan QRIS masing-masing
- 🎨 **Desain Responsif** - optimal di mobile dan desktop  
- 🌈 **Warna Unik** per lapak untuk mudah dibedakan
- ⚡ **Loading Cepat** - optimized untuk performa tinggi
- 📖 **Petunjuk Lengkap** cara scan QRIS
- 🆓 **Hosting Gratis** di GitHub Pages

## 🏪 Lapak yang Tersedia

1. **Cunah Culinary** (Bu Cunah) - Masakan rumahan berkualitas tinggi
2. **Dapur Runa** (Mbak Runa) - Katering sehat dan bergizi  
3. **Harumsari** (Pak Harum) - Warung kopi dan cemilan tradisional
4. **Minibul** (Mbak Mini) - Toko kelontong mini serbaguna
5. **Pawon Nyai** (Nyai Sari) - Dapur tradisional cita rasa autentik

## 🛠️ Teknologi

- **HTML5** dengan semantic markup
- **Tailwind CSS** via CDN untuk styling
- **Google Fonts** (Poppins) untuk tipografi
- **JavaScript ES6+** untuk dynamic content loading
- **JSON** untuk data management
- **Responsive Design** dengan CSS Grid dan Flexbox
- **GitHub Pages** ready untuk hosting

## 📊 Struktur Data JavaScript

Data lapak disimpan dalam variabel `shopsData` di dalam file `index.html`:

```javascript
const shopsData = {
  "shops": [
    {
      "id": "shop-id",
      "name": "Nama Lapak",
      "owner": "Nama Pemilik",
      "description": "Deskripsi lapak",
      "products": ["Produk 1", "Produk 2"],
      "qrisImage": "img/shop-qris.jpeg",
      "whatsappNumber": "+628123456789",
      "colorTheme": {
        "bg": "bg-blue-100",
        "border": "border-blue-200",
        "icon": "bg-blue-500",
        "tag": "bg-blue-200 text-blue-800",
        "text": "text-blue-700",
        "button": "bg-blue-500 hover:bg-blue-600",
        "imageBorder": "border-blue-300"
      }
    }
  ]
};
```

## 🚀 Cara Deploy ke GitHub Pages

1. Push semua file ke repository GitHub
2. Masuk ke Settings → Pages  
3. Pilih source "Deploy from a branch"
4. Pilih branch `main` dan folder `/ (root)`
5. Website akan tersedia di `https://username.github.io/khalayak-luwe`

## 📱 Cara Menggunakan

1. Buka website di browser
2. Pilih lapak yang ingin dibayar
3. Scan QRIS menggunakan aplikasi e-wallet atau Google Lens
4. Masukkan nominal dan konfirmasi pembayaran

## 📁 Struktur File

```
khalayak-luwe/
├── index.html              # Halaman utama (dengan data embedded)
├── img/                    # Folder gambar QRIS
│   ├── cunah-culinary.jpeg
│   ├── dapur-runa.jpeg  
│   ├── harumsari.jpeg
│   ├── minibul.jpeg
│   └── pawon-nyai.jpeg
├── README.md               # Dokumentasi proyek
└── Khalayak_Luwe_Youniverse_PRD.md  # Product Requirements Document
```

## 🎨 Design System

- **Font**: Poppins (Google Fonts)
- **Warna Utama**: Gray-50 background, Gray-800 text
- **Warna Lapak**: Product-based themes - Orange (snacks), Emerald (meals), Amber (coffee), Red (spicy), Pink (sweets)
- **Radius**: rounded-xl untuk card
- **Shadow**: md dengan hover:lg
- **Transition**: 300ms untuk smooth interaction

## 📊 Performance

- Total size < 1MB (sesuai PRD requirement)
- Loading time < 2 detik di mobile
- Optimized images dengan proper alt text
- SEO friendly dengan meta tags

## 🤝 Kontribusi

Untuk menambah lapak baru:
1. Tambahkan gambar QRIS di folder `img/`
2. Edit variabel `shopsData` di dalam file `index.html`
3. Tambahkan objek lapak baru ke dalam array `shops`
4. Ikuti struktur data yang sudah ada dengan ID unik
5. Pilih warna theme yang berbeda dari yang sudah ada
6. Website akan otomatis memuat data baru

## 📄 Lisensi

Proyek ini dibuat untuk mendukung UMKM lokal.  
© 2024 Agus Salim & Friends

---

💙 **Terima kasih telah mendukung UMKM lokal!**
