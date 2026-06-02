# Contributing to Financeku

Terima kasih telah tertarik untuk berkontribusi pada Financeku! 🎉

## Bagaimana Cara Berkontribusi?

### 1. Fork & Clone Repository
```bash
# Fork repository di GitHub
# Lalu clone fork Anda
git clone https://github.com/YOUR_USERNAME/Financeku.git
cd Financeku
```

### 2. Buat Branch Feature
```bash
git checkout -b feature/nama-fitur-anda
# atau untuk bug fix
git checkout -b fix/deskripsi-bug
```

### 3. Buat Perubahan
- Edit file yang diperlukan
- Test perubahan di berbagai browser
- Pastikan tidak ada error di console

### 4. Commit & Push
```bash
git add .
git commit -m "feat: Deskripsi singkat perubahan"
git push origin feature/nama-fitur-anda
```

### 5. Buat Pull Request
- Buka GitHub repository original
- Klik "New Pull Request"
- Pilih branch Anda dan tuliskan deskripsi detail

## Commit Message Convention

Gunakan format berikut:
- `feat:` - Fitur baru
- `fix:` - Bug fix
- `docs:` - Dokumentasi
- `style:` - Formatting, missing semicolons, dll
- `refactor:` - Kode refactoring tanpa perubahan fitur
- `test:` - Testing
- `ci:` - CI/CD changes

**Contoh:**
```
feat: Tambah fitur recurring transactions
fix: Perbaiki bug calculation di budget tracker
docs: Update README dengan deployment guide
```

## Development Guidelines

### Code Style
- Gunakan variable names yang deskriptif
- Tambahkan comments untuk logika kompleks
- Indentation: 2 spaces (bukan tabs)

### Testing Requirement
Sebelum submit PR:
- ✅ Test di Chrome, Firefox, Safari, Edge
- ✅ Test di mobile (gunakan DevTools)
- ✅ Tidak ada console errors/warnings
- ✅ Local Storage berfungsi dengan baik

### Documentation
- Update README jika ada perubahan fitur besar
- Dokumentasikan kategori/dompet baru yang ditambahkan
- Jelaskan perubahan di PR description

## Type of Contributions

### 🐛 Bug Reports
Buat issue dengan:
- Deskripsi bug yang jelas
- Steps to reproduce
- Browser & OS yang digunakan
- Expected vs actual behavior

### 💡 Feature Requests
Buat issue/discussion dengan:
- Deskripsi fitur
- Use case & manfaatnya
- Mockup atau sketsa (opsional)

### 📝 Documentation
- Grammar & typo fixes
- Update guides & tutorials
- Improve clarity

### 🎨 UI/UX Improvements
- Design improvements
- Better mobile responsiveness
- Accessibility improvements

## Area untuk Kontribusi

**Backend/Logic:**
- Optimasi perhitungan budget
- Improve formula kategori spending
- Add validation untuk input

**Frontend:**
- Add dark mode toggle
- Improve mobile UI
- Add animations/transitions
- Better chart visualizations

**Features:**
- Multi-currency support
- Recurring transactions
- Data import/export
- Cloud sync preparation

**Testing & Quality:**
- Browser compatibility testing
- Performance optimization
- Accessibility audit

## Questions?

- 💬 Open GitHub Discussions
- 📧 Contact melalui GitHub profile
- 🐛 Check existing issues terlebih dahulu

---

**Selamat berkontribusi! 🚀**
