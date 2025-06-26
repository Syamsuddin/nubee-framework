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
/nubee-framework/
├── index.php                   # Entry point: routing dan load layout
│
├── classes/
│   ├── auth.php                # Class Auth: login/logout, proteksi session
│   ├── category.php		 # Class categori
│   ├── config.php              # Konfigurasi database dan konstanta global
│   ├── csrf.php                # Class CSRF: proteksi anti-CSRF
│   ├── menu.php                # Class Menu: menu, submenu, dan akses role
│   ├── Postingan.php		 # Class Postingan
│   ├── session_security.php    # Class SessionSecurity: validasi IP/user agent
│   └── user.php                # Class User: CRUD user
│
├── layout/
│   ├── header.php              # Bagian atas halaman: menu, HTML head
│   ├── content.php             # Konten utama (berubah-ubah berdasarkan page)
│   └── footer.php              # Bagian bawah halaman
│
├── pages/
│   ├── dashboard.php           # Halaman utama pengguna setelah login
│   ├── login.php               # Form login pengguna
│   ├── user-list.php           # Daftar user (contoh CRUD)
│   ├── menu-builder.php        # Manajemen menu dan akses (opsional)
│   └── error.php               # Halaman error (403, 404)
│
├── public/
│   ├── landing.php             # Halaman landing aplikasi
│   ├── login.php               # Form login pengguna
│   ├── 403.php        		 # Halaman error 403
│   └── 404.php               	 # Halaman error 404
│
├── assets/
│   ├── css/
│   │   └── style.css           # Style utama aplikasi
│   ├── js/
│   │   └── app.js              # Script interaktif jika ada
│   └── img/
│       └── logo.png            # Logo aplikasi
│
├── uploads/                    # (Opsional) Tempat penyimpanan file upload
├── db.sql               	 # File struktur tabel database Nubee
├── dokumentasi.pdf             # File dokumentasi Nubee framwork
└── README.md                   # Dokumentasi dan petunjuk penggunaan

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
