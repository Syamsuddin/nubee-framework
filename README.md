# Nubee Framework

**Nubee Framework** adalah mini-framework PHP native yang ringan, aman, dan modular, dirancang untuk mempercepat dan menyederhanakan proses pengembangan aplikasi web skala kecil-menengah.

Framework ini menghadirkan routing URL dinamis, sistem login & manajemen sesi yang aman, hak akses berbasis role, serta CMS sederhana menggunakan konsep post dan slug. Nubee Framework cocok digunakan untuk aplikasi pemerintahan, sistem informasi desa, sekolah, hingga dashboard administratif.

## Fitur Utama

* Routing modular dan aman
* Otentikasi pengguna dan keamanan sesi
* Role-based access control (RBAC)
* Menu dinamis otomatis dari database
* CMS sederhana (post dan slug)
* Perlindungan keamanan tambahan (CSRF, validasi input, logging aktivitas)

## Struktur Folder

```
nubee-framework/
├── index.php
├── classes/
│   ├── auth.php
│   ├── config.php
│   ├── csrf.php
│   ├── menu.php
│   ├── postingan.php
│   ├── session_security.php
│   └── user.php
├── pages/
│   ├── public/
│   └── cms/
└── layout/
    ├── header.php
    ├── content.php
    └── footer.php
```

## Instalasi

1. Clone repository ini:

```bash
git clone https://github.com/username/nubee-framework.git
```

2. Konfigurasi database di `classes/config.php`

3. Import struktur database dari file yang tersedia

4. Jalankan aplikasi melalui server lokal seperti XAMPP atau web server lainnya.

## Lisensi

Nubee Framework tersedia dalam lisensi MIT. Silakan gunakan dan kembangkan sesuai kebutuhan proyek Anda.
