# 💰 Financeku - Personal Finance Manager

Aplikasi manajemen keuangan pribadi berbasis web yang intuitif dan powerful. Catat transaksi, kelola budget, pantau tabungan, dan lihat analisis keuangan Anda dalam satu dashboard yang cantik.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Deploy Status](https://img.shields.io/badge/Deploy-Vercel-success)](https://financeku-taupe.vercel.app)
![HTML](https://img.shields.io/badge/HTML-5-E34C26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?logo=javascript&logoColor=black)

**Live Demo:** https://financeku-taupe.vercel.app

---

## ✨ Fitur Utama

### 📊 Dashboard Interaktif
- Ringkasan saldo total, pemasukan, dan pengeluaran
- Grafik tren pemasukan vs pengeluaran (6 bulan terakhir)
- Widget dompet, anggaran, dan utang dalam satu layar
- Periode filter: Bulan, Minggu, Tahun

### 💳 Manajemen Dompet
- Daftar saldo bank, tunai, dan e-wallet
- Komposisi dompet dengan visualisasi persentase
- Support: BCA, DANA, OVO, Tunai, dan lebih banyak

### 💸 Pencatatan Transaksi
- Tambah transaksi pemasukan dan pengeluaran
- Kategorisasi otomatis
- Tautan ke berbagai dompet
- Search dan filter transaksi
- Catatan tambahan untuk setiap transaksi

### 💰 Manajemen Budget
- Set limit anggaran per kategori
- Real-time tracking vs realisasi
- Warning otomatis ketika mendekati atau melebihi limit
- Status kategori untuk monitoring

### 🏦 Tabungan & Target
- Buat target finansial dengan deadline
- Track progress pencapaian target
- Visualisasi dengan progress bar
- Total dana tersimpan vs target

### 📋 Utang & Piutang
- Catat utang yang perlu dilunasi
- Catat piutang yang akan diterima
- Status tracking (Belum lunas / Lunas / Menunggu)
- Tanggal jatuh tempo untuk reminder

### 📈 Analisis & Laporan
- KPI dashboard: Total pemasukan, pengeluaran, arus kas bersih
- Pengeluaran per kategori
- Aktivitas transaksi terbaru
- Export ringkasan laporan
- Grafik tren bulanan dan komposisi kategori

### 📱 Responsive Design
- Fully responsive untuk desktop, tablet, dan mobile
- Sidebar navigation yang collapses di mobile
- Touch-friendly interface

---

## 🚀 Cara Menggunakan

### Quick Start
1. Buka https://financeku-taupe.vercel.app di browser
2. Mulai gunakan langsung tanpa instalasi!

### Fitur Utama Dashboard
- **Tambah Transaksi**: Klik tombol "Tambah" untuk mencatat pemasukan/pengeluaran
- **Switch View**: Gunakan sidebar untuk navigasi antar halaman (Dashboard, Transaksi, Dompet, dll)
- **Filter Data**: Gunakan search dan dropdown filter untuk mencari transaksi spesifik
- **Export Laporan**: Di halaman Laporan, klik "Export ringkasan" untuk CSV

### Kategori Default
**Pemasukan:** Gaji, Freelance, Bonus, Investasi, Penjualan

**Pengeluaran:** Makan, Transport, Belanja, Tagihan, Hiburan, Kesehatan, Pendidikan

---

## 💻 Development Setup

### Prerequisites
- Web browser modern (Chrome, Firefox, Safari, Edge)
- Text editor (VS Code, Sublime, dll)

### Installation
```bash
# Clone repository
git clone https://github.com/Coda-ku/Financeku.git
cd Financeku

# Buka di browser
open index.html
# atau cukup drag-drop index.html ke browser
```

### Struktur Project
```
Financeku/
├── index.html                              # Main aplikasi (all-in-one)
├── personal_finance_manager_dashboard.html # Alternative version
├── README.md                               # Dokumentasi ini
└── .github/
    └── workflows/
        └── deploy.yml                      # CI/CD configuration
```

### Tech Stack
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Charts**: Chart.js v4.4.0
- **Icons**: Tabler Icons
- **Fonts**: Inter (Google Fonts)
- **Hosting**: Vercel
- **Storage**: Local Storage (Browser)

---

## 🔧 Konfigurasi

### Data Storage
Data disimpan di **Local Storage** browser. Data akan persisten selama:
- ✅ Browser history tidak dihapus
- ✅ Website di-bookmark atau dikunjungi kembali
- ❌ Clear browser cache akan menghapus semua data

### Environment Setup
Tidak ada file `.env` diperlukan - aplikasi fully static.

### Customization

#### Menambah Kategori Baru
Edit di `index.html` lines 675-676:
```javascript
const incomeCategories = ['Gaji','Freelance','Bonus','Investasi','Penjualan','YOUR_CATEGORY']
const expenseCategories = ['Makan','Transport','Belanja','Tagihan','Hiburan','Kesehatan','Pendidikan','YOUR_CATEGORY']
```

#### Menambah Dompet
Edit data `wallets` di lines 684-689:
```javascript
let wallets = [
  { id:'bca', icon:'ti-building-bank', cls:'w-dark', name:'Rekening BCA', type:'Bank', bal:4250000 },
  // Tambah di sini
  { id:'new', icon:'ti-icon-name', cls:'w-color', name:'Nama Dompet', type:'Tipe', bal:0 }
]
```

#### Mengubah Warna & Tema
CSS custom properties di lines 13-20:
```javascript
:root{
  --dark:#0D0D0D;           // Primary color
  --up:#1D9E75;             // Income/positive color
  --down:#E24B4A;           // Expense/negative color
  --warn:#BA7517;           // Warning color
  --info:#185FA5;           // Info color
  // ... dan lainnya
}
```

---

## 📊 API & Integrasi

### Planned Features
- [ ] WhatsApp Integration - Notifikasi transaksi via WA
- [ ] Cloud Sync - Auto backup data ke cloud
- [ ] Mobile App - Native app untuk iOS & Android
- [ ] Recurring Transactions - Transaksi otomatis
- [ ] Receipt OCR - Scan invoice & receipt
- [ ] Budget Recommendations - AI suggestions

### Roadmap
Fitur-fitur yang sedang dikembangkan untuk rilis berikutnya:

| Feature | Status | ETA |
|---------|--------|-----|
| WhatsApp Bot | 🔄 In Progress | Q3 2026 |
| Multi-currency | 📋 Planned | Q3 2026 |
| Data Export (PDF/Excel) | 📋 Planned | Q2 2026 |
| Dark Mode Toggle | 📋 Planned | Q2 2026 |
| Mobile App | 📋 Planned | Q4 2026 |

---

## 🚀 Deployment

### Deploy ke Vercel (Recommended)
```bash
# 1. Push ke GitHub
git push origin main

# 2. Connect repository ke Vercel
# Kunjungi https://vercel.com dan import GitHub repo
# Vercel akan auto-deploy setiap push ke main

# 3. Custom domain (optional)
# Setup di Vercel dashboard
```

### Deploy ke GitHub Pages
```bash
# 1. Update repository settings
# Go to Settings > Pages > Source: Deploy from branch > main

# 2. Push ke main
git push origin main

# Website akan live di https://coda-ku.github.io/Financeku
```

### Deploy ke Netlify
```bash
# 1. Drag & drop folder ke Netlify
# atau connect GitHub repository
```

---

## 📝 Browser Support

| Browser | Version | Support |
|---------|---------|---------|
| Chrome | Latest | ✅ Full |
| Firefox | Latest | ✅ Full |
| Safari | Latest | ✅ Full |
| Edge | Latest | ✅ Full |
| IE 11 | - | ❌ Not Supported |

---

## 🤝 Contributing

Kami menerima kontribusi! Bagaimana cara berkontribusi:

1. Fork repository ini
2. Buat branch fitur (`git checkout -b feature/AmazingFeature`)
3. Commit perubahan (`git commit -m 'Add AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buka Pull Request

### Development Guidelines
- Jaga code style konsisten
- Tambah comments untuk logika kompleks
- Test di berbagai browser sebelum PR
- Update README jika ada perubahan fitur

---

## 🐛 Known Issues

- Local Storage terbatas ~5-10MB tergantung browser
- Data bersifat lokal dan tidak tersinkronisasi antar device
- Grafik Chart.js membutuhkan internet untuk cdn.jsdelivr.net

---

## 📄 License

Project ini dilisensikan di bawah MIT License - lihat file [LICENSE](LICENSE) untuk detail.

---

## 👨‍💻 Author

**Coda-ku** - [@Coda-ku](https://github.com/Coda-ku)

---

## 📞 Support & Feedback

- 🐛 **Bug Report**: [GitHub Issues](https://github.com/Coda-ku/Financeku/issues)
- 💡 **Feature Request**: [GitHub Discussions](https://github.com/Coda-ku/Financeku/discussions)
- 📧 **Email**: Hubungi melalui GitHub profile

---

## 🙏 Terima Kasih

Terima kasih kepada:
- [Chart.js](https://www.chartjs.org/) - Chart library
- [Tabler Icons](https://tabler-icons.io/) - Icon set
- [Google Fonts](https://fonts.google.com/) - Inter typeface
- [Vercel](https://vercel.com/) - Hosting & deployment

---

**Made with ❤️ by Coda-ku**

Jika project ini membantu, jangan lupa ⭐ di GitHub!
