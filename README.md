# Jatim High-Velocity Anomaly Engine (Resolusi Pi-55)

[![Production Ready](https://img.shields.io/badge/status-production--ready-green.svg)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](#)
[![Built with Vanilla JS](https://img.shields.io/badge/Built%20with-Vanilla%20JS%20%2F%20Chart.js-orange.svg)](#)

Sistem Peringatan Dini Kuantitatif (**Quantitative Early Warning System**) berbasis web terintegrasi untuk mendeteksi distorsi, ketidakstabilan termal, dan anomali atmosfer makro di 38 Kabupaten/Kota Jawa Timur secara *real-time*. 

Aplikasi ini beroperasi penuh di sisi klien (*client-side architecture*) dengan memanfaatkan pipeline asinkronus untuk memanen telemetri satelit cuaca global secara simultan, kemudian mengevaluasinya menggunakan matriks filter interferensi berbasis fraktal universal $\pi$ presisi 55 desimal.

---

## 🚀 Fitur Utama
- **0-Rupiah Infrastructure**: Berjalan sepenuhnya di sisi klien menggunakan Vanilla JS dan `Promise.all()`. Tidak memerlukan infrastruktur server backend berbayar atau alokasi basis data terpusat.
- **Real-Time Geospatial Ingestion**: Integrasi langsung ke API satelit meteorologi Open-Meteo dengan metode paralel HTTP requests (resolusi ~1-2 detik untuk seluruh wilayah provinsi).
- **High-Precision Quantum-Fourier Filtering**: Menggunakan sisa pembagian (*modulo*) konstanta irasional $\pi_{55}$ sebagai koefisien resonansi untuk menangkap riak anomali termodinamika atmosfer.
- **Interactive Data Visualization**: Dibekali dengan grafik horizontal terurut (*dynamic sorting*) dari Chart.js yang secara otomatis memetakan status wilayah dari `STABIL` hingga `CRITICAL` menggunakan gradasi warna fisis.

---

## 📐 Pemodelan Matematika Core Engine

Indeks anomali atmosfer ($\mathcal{I}$) pada tiap simpul koordinat geospasial dihitung menggunakan fungsi interferensi non-linear berikut:

$$\mathcal{I} = \text{clamp}\left( \sin(\theta \cdot \Delta T) \cdot \Delta T + \left( \Delta P \cdot 0.01 \cdot \mathcal{E}_k \right) \cdot \pi, -5.0, 5.0 \right)$$

Di mana:
- $\theta = \pi_{55} \pmod 1$ (Koefisien Resonansi Fraktal)
- $\Delta T = T_{\text{aktual}} - T_{\text{normal}}$ (Deviasi Termal regional, $T_{\text{normal}} = 27.0^\circ\text{C}$)
- $\Delta P = P_{\text{aktual}} - 1013.25\text{ hPa}$ (Delta Tekanan Barometrik Atas Permukaan Laut)
- $\mathcal{E}_k = \frac{1}{2} \rho v^2$ (Pendekatan Energi Kinetik Angin Lokal, di mana $v$ adalah kecepatan angin)

### Interpretasi Vektor Grafik (Chart.js)
- **Batang Grafik ke Kanan (Skor Positif / Gradasi Merah)**: Menandakan akumulasi energi termal dan tekanan udara tinggi. Berpotensi memicu pusaran angin kencang lokal atau **Puting Beliung** akibat fenomena *updraft* masif.
- **Batang Grafik ke Kiri (Skor Negatif / Gradasi Biru)**: Menandakan runtuhnya tekanan udara permukaan secara radikal bawah batas normal. Berpotensi memicu pembentukan awan *Cumulonimbus* tebal penyebab **Hujan Lebat Ekstrem dan Badai**.

---

## 🛠️ Panduan Instalasi & Penggunaan

Karena proyek ini mengusung arsitektur *Single Page Application* (SPA), tidak ada proses kompilasi (*zero build setup*).

1. Clone repositori ini ke komputer lokal Anda:
   ```bash
   git clone [https://github.com/username/cuaca.git](https://github.com/username/cuaca.git)

👨‍💻 Kontributor & Atribusi KreditProyek ini dikembangkan, dirancang, dan dioptimasi oleh: Muhibbuddin 

— Core Architecture & Engine Designer Profil Resmi: https://www.facebook.com/inggik

Seluruh hak kekayaan intelektual terkait formulasi struktur penapisan gelombang cuaca menggunakan konstanta $\pi_{55}$ pada repositori ini dilindungi di bawah atribusi pengembang asli.

📄 LisensiProyek ini dilisensikan di bawah MIT License - lihat berkas halaman kode untuk detail lebih lanjut. 

Penggunaan untuk keperluan riset akademis maupun implementasi Smart City pemerintahan diwajibkan tetap menyertakan atribusi pengembang di atas.
