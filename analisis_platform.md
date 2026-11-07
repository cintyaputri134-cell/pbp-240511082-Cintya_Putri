# Analisis Platform: Web, Desktop, & Mobile

Laporan Komparatif Arsitektur dan Karakteristik Pengembangan Perangkat Lunak.

## 1. Pendahuluan

Dalam rekayasa perangkat lunak modern, pemilihan platform (Web, Desktop, atau Mobile) merupakan keputusan arsitektural krusial yang menentukan jangkauan pengguna, performa, kompleksitas pengembangan, serta biaya pemeliharaan. Dokumen ini menyajikan analisis komprehensif mengenai perbandingan ketiga platform tersebut berdasarkan berbagai aspek teknis dan operasional.

## 2. Tabel Perbandingan Platform

| Aspek | Web | Desktop | Mobile |
| :--- | :--- | :--- | :--- |
| **Arsitektur** | Client-Server (Browser-based, Single Page Application / Progressive Web App) | Standalone Application (Native binary, Client-heavy, Local Database/File System) | Mobile Native / Hybrid / Cross-Platform (Sandboxed execution, App Sandbox & OS APIs) |
| **Bahasa Utama** | HTML, CSS, JavaScript / TypeScript, PHP, Python | Java (Swing/JavaFX), C#, C++, Python, JavaScript (Electron) | Kotlin, Swift, Java, Dart (Flutter), JavaScript/TypeScript (React Native) |
| **Distribusi** | Deployment melalui web server / cloud hosting; dapat diakses instan via URL tanpa instalasi. | Distribusi file installer (`.exe`, `.dmg`, `.deb`, `.msi`) atau melalui Microsoft Store / Mac App Store. | Distribusi terpusat melalui Official App Stores (Google Play Store, Apple App Store). |
| **Keunggulan** | Cross-platform universal, tidak perlu instalasi, mudah diperbarui secara terpusat (CI/CD). | Performa tinggi, akses penuh ke hardware lokal, bekerja optimal secara offline. | Mobilitas tinggi, integrasi sensor perangkat (GPS, Kamera, Biometrik), notifikasi push real-time. |
| **Keterbatasan** | Ketergantungan pada koneksi internet, keterbatasan akses hardware device secara mendalam. | Proses distribusi update manual atau butuh mekanisme auto-update khusus; terikat OS spesifik. | Ukuran layar terbatas, fragmentasi perangkat/OS yang tinggi, proses review store yang ketat. |
| **Contoh Aplikasi** | GitHub, Google Workspace, Smart Tourism WebGIS (Leaflet.js) | Visual Studio Code, XAMPP Control Panel, Aplikasi Kasir (POS) | WhatsApp, Instagram, Mobile Banking (BSI / BCA Mobile) |

## 3. Evaluasi Mendalam & Rekomendasi

### Kapan Memilih Platform Web?
Platform web sangat ideal untuk aplikasi yang membutuhkan jangkauan luas tanpa hambatan instalasi, kolaborasi real-time, serta pembaruan sistem yang sering dan terpusat. Cocok untuk sistem informasi, portal berita, e-commerce, dan dashboard analitik berbasis cloud.

### Kapan Memilih Platform Desktop?
Aplikasi desktop dipilih ketika performa komputasi berat, pemrosesan data lokal berukuran masif, atau akses langsung ke perangkat keras (*hardware/peripheral*) menjadi prioritas utama, seperti software editor video, IDE, sistem ERP enterprise lokal, dan game berat.

### Kapan Memilih Platform Mobile?
Platform mobile wajib digunakan ketika produk berfokus pada mobilitas pengguna harian, pemanfaatan fitur sensor smartphone (GPS untuk pelacakan, kamera untuk pemindaian, sensor sidik jari), serta keterlibatan pengguna (*user engagement*) melalui sistem *push notification*.

---
**Kesimpulan:** Pemilihan arsitektur platform tidak harus eksklusif. Pendekatan modern sering kali menggabungkan ketiganya melalui API backend yang sama (*multi-platform ecosystem*) untuk memaksimalkan pengalaman pengguna di berbagai perangkat.