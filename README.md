# CyberRoute: The Network Architect 🌐

> **Media Pembelajaran APE (Alat Permainan Edukatif) Plugged Interaktif**  
> Mata Pelajaran: Informatika (Fase F - Kelas XI SMA/SMK)  
> Elemen: Jaringan Komputer dan Internet (JKI) & Arsitektur Topologi Jaringan

---

## 🎯 Gambaran Umum Proyek

**CyberRoute** adalah simulator interaktif berbasis web yang memadukan konsep topologi jaringan komputer nyata dengan mekanisme permainan berbasis pemecahan masalah (*problem-based learning*). Dikembangkan dengan pendekatan desain antarmuka bersih tanpa ketergantungan aset eksternal dan bebas dari karakter emoji tipikal AI, menghadirkan estetika teknis bergaya konsol operasi jaringan (*Network Operations Console*).

### Fitur Utama:
1. **Interactive Magnetic Port Snapping Canvas**:
   - Tarik dan hubungkan kabel antar simpul jaringan (*workstation*, *central hub/server*, *bus node*, *firewall gateway*, dll).
   - Pengukuran jarak dan batas anggaran kabel (*cable budget*) secara akurat dan real-time.
2. **Evaluasi Topologi Otomatis & Pathfinding**:
   - Algoritma penelusuran graf (*BFS Shortest Path*) yang secara cerdas mendeteksi bentuk topologi:
     - **Topologi Star**: Verifikasi hubungan klien langsung ke konsentrator pusat dan uji *Fault Isolation* serta simulasi *Single Point of Failure (SPOF)*.
     - **Topologi Bus**: Verifikasi rantai linier *backbone* dan uji *Binary Troubleshooting* saat terjadi putus jalur.
     - **Topologi Mesh (Partial)**: Rute primer berkecepatan tinggi dengan cadangan *Dynamic Failover* untuk mencapai kondisi *Zero Packet Drop*.
     - **Topologi Hybrid (Boss Level)**: Gabungan koridor industri, fasilitas medis, dan pusat data dalam skenario darurat dengan batas waktu *Time To Live (TTL)*.
3. **Audio Synthesizer Mandiri (Web Audio API)**:
   - Sintesis audio prosedural tanpa file eksternal (suara klik, koneksi kabel, laser glitch, dan konfirmasi keberhasilan).
4. **Instrumen LKPD Terintegrasi**:
   - Refleksi konseptual terstruktur untuk setiap level dan tombol unduh laporan praktikum (`.txt`) untuk penilaian guru/dosen.
5. **Responsif & Kompatibel Layar Sentuh**:
   - Dukungan penuh untuk mouse dan sentuhan layar (*touch gestures*) pada tablet/Chromebook siswa.

---

## 🚀 Cara Menjalankan Secara Lokal

Cukup buka berkas `index.html` di peramban web modern manapun, atau jalankan server lokal:

```bash
# Menggunakan Python
python -m http.server 8000

# Atau menggunakan Node.js
npx serve .
```

Buka peramban di [http://localhost:8000](http://localhost:8000).

---

## 🌐 Deployment & Hosting

Proyek ini telah dikonfigurasi untuk langsung aktif pada:
- **GitHub Pages**: Dikelola secara otomatis melalui alur kerja GitHub Actions pada `.github/workflows/deploy.yml`.
- **URL Publik GitHub Pages**: `https://fedoraard.github.io/cyberroute/`

---

## 🛠 Lisensi & Kontributor

Dikembangkan untuk kebutuhan perkuliahan/pembelajaran Informatika & Media Permainan Edukatif.
Repositori: [https://github.com/Fedoraard/cyberroute](https://github.com/Fedoraard/cyberroute)
