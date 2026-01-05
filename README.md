# 📚 Dokumentasi Aplikasi Kurir SiAktif

<div align="center">

[![Documentation](https://img.shields.io/badge/docs-live-success?style=for-the-badge&logo=readthedocs&logoColor=white)](https://denis156.github.io/siaktif-documentation/)
[![MkDocs](https://img.shields.io/badge/MkDocs-Material-blue?style=for-the-badge&logo=materialformkdocs&logoColor=white)](https://squidfunk.github.io/mkdocs-material/)
[![License](https://img.shields.io/badge/License-Proprietary-red?style=for-the-badge)](#)

</div>

Dokumentasi lengkap untuk aplikasi kurir laundry SiAktif - Platform digital yang memudahkan kurir dalam mengelola pesanan, navigasi, dan komunikasi dengan admin & pelanggan.

## 🚀 Live Documentation

**📖 Akses dokumentasi online:** **[https://denis156.github.io/siaktif-documentation/](https://denis156.github.io/siaktif-documentation/)**

Dokumentasi di-deploy otomatis menggunakan GitHub Actions setiap kali ada perubahan di branch `main`.

## 🌟 Tentang Proyek

Dokumentasi ini dibuat menggunakan **[MkDocs Material](https://squidfunk.github.io/mkdocs-material/)** dengan desain modern, responsif, dan user-friendly. Dokumentasi ini ditujukan untuk membantu kurir memahami dan menggunakan aplikasi SiAktif dengan maksimal.

### ✨ Fitur Dokumentasi

- 🎨 **Modern UI** - Material Design theme dengan dark mode
- 📱 **Responsif** - Tampil sempurna di desktop, tablet, dan mobile
- 🔍 **Search** - Pencarian cepat dengan autocomplete
- 🌙 **Dark Mode** - Toggle antara light/dark theme
- 📴 **Offline Support** - Bisa diakses tanpa internet setelah pertama kali dibuka
- 🗺️ **Navigasi Intuitif** - Tabs, breadcrumbs, dan table of contents
- 💬 **Interactive** - Grid cards, admonitions, tabs, dan code blocks

## 📸 Preview

Kunjungi [Live Documentation](https://denis156.github.io/siaktif-documentation/) untuk melihat tampilan lengkap dokumentasi.

**Fitur Unggulan:**
- ✨ Grid cards dengan Material icons
- 🎨 Admonitions untuk highlight informasi penting
- 📑 Content tabs untuk konten alternatif
- 🌙 Dark mode support
- 📱 Fully responsive design

## 🛠️ Tech Stack

- **[MkDocs](https://www.mkdocs.org/)** - Static site generator
- **[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)** - Material Design theme
- **[Python Markdown Extensions](https://facelessuser.github.io/pymdown-extensions/)** - Extended Markdown features

## 📋 Prasyarat

Pastikan kamu sudah install:

- Python 3.8 atau lebih baru
- pip (Python package manager)

## 🚀 Quick Start

### 1. Install Dependencies

```bash
# Install MkDocs Material
brew install mkdocs-material

# Atau via pip
pip install mkdocs-material
```

### 2. Clone Repository

```bash
git clone https://github.com/denis156/siaktif-documentation.git
cd siaktif-documentation
```

### 3. Jalankan Development Server

```bash
mkdocs serve
```

Buka browser dan akses: **http://127.0.0.1:8000**

### 4. Build untuk Production

```bash
mkdocs build
```

File hasil build akan ada di folder `site/`

## 📁 Struktur Proyek

```
siaktif/
├── docs/                          # Source documentation files
│   ├── images/                    # Screenshots & assets
│   │   ├── instalasi/
│   │   ├── navigasi/
│   │   ├── menu-utama/
│   │   ├── jemput-antar/
│   │   ├── navigasi-rute/
│   │   ├── chat/
│   │   └── profile/
│   ├── menu-utama/                # Menu utama pages
│   │   ├── beranda.md
│   │   ├── aktifitas.md
│   │   ├── rute.md
│   │   ├── chat.md
│   │   └── pengaturan.md
│   ├── panduan-fitur/             # Feature guides
│   │   ├── jemput-pesanan.md
│   │   ├── antar-pesanan.md
│   │   ├── upload-bukti.md
│   │   ├── navigasi-rute.md
│   │   ├── menggunakan-chat.md
│   │   └── edit-profile.md
│   ├── index.md                   # Homepage
│   ├── instalasi.md               # Installation guide
│   ├── autentikasi.md             # Authentication guide
│   ├── navigasi.md                # Navigation guide
│   ├── tips-trik.md               # Tips & tricks
│   └── faq.md                     # FAQ
├── mkdocs.yml                     # MkDocs configuration
└── README.md                      # This file
```

## ⚙️ Konfigurasi

File konfigurasi utama ada di `mkdocs.yml`. Beberapa hal yang bisa dikustomisasi:

- **Theme colors** - Primary & accent colors
- **Navigation** - Menu structure
- **Features** - Enable/disable features
- **Extensions** - Markdown extensions
- **Plugins** - Additional functionality

## 📝 Cara Mengedit Dokumentasi

1. Buka file `.md` yang ingin diedit di folder `docs/`
2. Edit menggunakan Markdown syntax
3. Simpan file
4. Development server akan auto-reload
5. Cek perubahan di browser

### Markdown Features yang Tersedia:

- **Admonitions** - Callout boxes (info, tip, warning, dll)
- **Grid Cards** - Card layout untuk features
- **Content Tabs** - Tabs untuk konten alternatif
- **Code Blocks** - Syntax highlighting
- **Material Icons** - `:material-icon-name:`
- **Mermaid Diagrams** - Flowcharts & diagrams
- **Task Lists** - Checklist items

Lihat [Material for MkDocs Documentation](https://squidfunk.github.io/mkdocs-material/reference/) untuk referensi lengkap.

## 🎨 Style Guidelines

### Material Icons
Gunakan Material icons, bukan emoji biasa:

```markdown
✅ BENAR: :material-home: :material-chat:
❌ SALAH: 🏠 💬
```

### Admonitions
Untuk highlight informasi penting:

```markdown
!!! info "Informasi"
    Konten informasi

!!! tip "Tips"
    Konten tips

!!! warning "Peringatan"
    Konten peringatan
```

### Grid Cards
Untuk layout features:

```markdown
<div class="grid cards" markdown>

-   :material-icon:{ .lg .middle } **Title**

    ---

    Description

</div>
```

## 🚢 Deployment

Dokumentasi ini menggunakan **GitHub Actions** untuk auto-deployment ke GitHub Pages.

### Automatic Deployment (Sudah Setup)

✅ CI/CD sudah dikonfigurasi di `.github/workflows/ci.yml`

Setiap kali ada push ke branch `main`, GitHub Actions akan:
1. Build dokumentasi menggunakan `mkdocs build`
2. Deploy otomatis ke branch `gh-pages`
3. Dokumentasi tersedia di: [https://denis156.github.io/siaktif-documentation/](https://denis156.github.io/siaktif-documentation/)

### Manual Deployment (Jika Diperlukan)

Jika ingin deploy manual:

```bash
# Build dan deploy ke GitHub Pages
mkdocs gh-deploy

# Atau build saja tanpa deploy
mkdocs build
```

### Setup GitHub Pages (First Time)

Jika baru pertama kali setup:

1. Push repository ke GitHub
2. Buka **Settings** → **Pages**
3. **Source**: Deploy from a branch
4. **Branch**: Pilih `gh-pages` → `/` (root)
5. Klik **Save**
6. Tunggu beberapa menit, docs akan live di `https://denis156.github.io/siaktif-documentation/`

## 🤝 Contributing

Kontribusi sangat diterima! Jika ingin berkontribusi:

1. Fork repository ini
2. Buat branch baru (`git checkout -b feature/AmazingFeature`)
3. Commit perubahan (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

### Reporting Issues

Jika menemukan bug atau punya saran:
- Buka issue di [GitHub Issues](https://github.com/denis156/siaktif-documentation/issues)
- Atau hubungi tim development via email

## 📞 Kontak

**PT. Aktif Gapura Internasional**

- 💬 **WhatsApp:** [+6282156912202](https://wa.me/6282156912202)
- 📧 **Email:** [support@aktiflaundry.com](mailto:support@aktiflaundry.com)
- 📱 **Instagram:** [@aktif_laundry](https://www.instagram.com/aktif_laundry/)
- 🌐 **Documentation:** [https://denis156.github.io/siaktif-documentation/](https://denis156.github.io/siaktif-documentation/)

## 📄 License

Copyright © 2026 PT. Aktif Gapura Internasional

---

<div align="center">

**Dibuat dengan ❤️ oleh Team SiAktif**

</div>
