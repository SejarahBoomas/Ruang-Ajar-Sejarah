# 📚 MPI Orde Baru & Reformasi — Panduan Pengembang

Media Pembelajaran Interaktif (MPI) Sejarah Fase F Kelas XII  
Topik: **Orde Baru dan Reformasi** — Dinamika Politik, Konflik & Identitas Bangsa

---

## 🗂️ Struktur Folder yang Diperlukan

Buat folder berikut di satu direktori dengan `index.html`:

```
📁 (root)
├── index.html          ← File utama MPI
├── README.md           ← Panduan ini
└── 📁 asset/
    ├── 📁 img/         ← Semua file gambar
    └── 📁 audio/       ← Semua file suara
```

---

## 🖼️ Daftar Aset Gambar yang Dibutuhkan (`./asset/img/`)

> ⚠️ Jika gambar tidak ada, MPI akan otomatis menampilkan **placeholder SVG berwarna** sehingga tetap bisa dijalankan.

### Gambar Utama (Hero & Background)
| Nama File | Ukuran Ideal | Keterangan |
|---|---|---|
| `bg_reformasi.jpg` | 1280×720 px | Latar belakang layar judul |
| `supersemar.jpg` | 640×400 px | Materi 1 — Supersemar |
| `dwifungsi.jpg` | 640×400 px | Materi 2 — Dwifungsi ABRI |
| `repelita.jpg` | 640×400 px | Materi 3 — Pembangunan Orba |
| `trisakti_demo.jpg` | 640×400 px | Materi 4 — Demo & Tragedi 1998 |
| `habibie_pemilu.jpg` | 640×400 px | Materi 5 — Habibie & Pemilu 1999 |
| `pilpres_langsung.jpg` | 640×400 px | Materi 6 — Pilpres 2004 |

### Foto Profil & Logo
| Nama File | Ukuran Ideal | Keterangan |
|---|---|---|
| `logo_sekolah.png` | 200×200 px | Logo institusi (transparan) |
| `profil_guru.jpg` | 300×380 px | Foto pengembang/guru |
| `raka.png` | 200×200 px | Avatar karakter Raka (transparan) |

### Gambar Tokoh (Aktivitas Bermain & Berlatih)
| Nama File | Ukuran Ideal | Keterangan |
|---|---|---|
| `elang.png` | 200×200 px | Elang Mulia Lesmana |
| `habibie_muda.png` | 200×200 px | B.J. Habibie |
| `megawati_muda.png` | 200×200 px | Megawati Soekarnoputri |
| `gus_dur.png` | 200×200 px | Abdurrahman Wahid |

### Ikon Game Jodoh (bisa icon flat sederhana)
| Nama File | Keterangan |
|---|---|
| `icon_orba.png` | Ikon era Orde Baru |
| `icon_ref1.png` | Ikon Reformasi awal |
| `icon_ref2.png` | Ikon Reformasi lanjutan |
| `icon_dok.png` | Ikon dokumen |
| `icon_bangunan.png` | Ikon pembangunan |
| `icon_militer.png` | Ikon militer/ABRI |
| `icon_pres3.png` | Ikon Presiden ke-3 |
| `icon_pres5.png` | Ikon Presiden ke-5 |

### Gambar Game Kumpul
| Nama File | Keterangan |
|---|---|
| `reformasi_tuntutan.png` | Gambar tuntutan reformasi (item BENAR) |
| `bukan_tuntutan1.png` | Gambar bukan tuntutan — item SALAH 1 |
| `bukan_tuntutan2.png` | Gambar bukan tuntutan — item SALAH 2 |

---

## 🔊 Daftar Aset Audio yang Dibutuhkan (`./asset/audio/`)

> ⚠️ Semua audio bersifat opsional. MPI tetap berjalan penuh tanpa audio.

| Nama File | Format | Keterangan |
|---|---|---|
| `bgm.mp3` | MP3, ~128kbps | Musik latar (looping) |
| `sfx_klik.mp3` | MP3, pendek | Efek suara klik tombol |
| `sfx_transisi.mp3` | MP3, pendek | Efek suara pindah layar |
| `sfx_bintang.mp3` | MP3, pendek | Efek suara selesai/menang |

---

## ⚙️ Cara Mengubah Konfigurasi

Buka `index.html`, cari bagian `const CFG = {` (sekitar baris 516), lalu ubah:

```javascript
const CFG = {
  judul: 'Orde Baru & Reformasi',         // Judul MPI
  subjudul: 'Dinamika Politik...',          // Sub-judul
  fase: 'Fase F · Kelas XII',              // Fase & Kelas
  mapel: 'Sejarah',                        // Mata pelajaran
  unit: 'Indonesia Modern',                // Unit
  subunit: 'Orde Baru dan Reformasi',      // Sub unit
  tp: 'Tujuan Pembelajaran...',            // Tujuan Pembelajaran
  logo: './asset/img/logo_sekolah.png',    // Path logo
  bgJudul: './asset/img/bg_reformasi.jpg', // Path background judul
  raka: './asset/img/raka.png',            // Path avatar Raka
  profil: {
    nama: 'Nama Lengkap Guru',             // ← UBAH INI
    instansi: 'Nama SMA / Instansi',       // ← UBAH INI
    jenis: 'Media Pembelajaran Interaktif (MPI)',
    foto: './asset/img/profil_guru.jpg'    // ← Path foto guru
  }
};
```

---

## 🎮 Fitur Lengkap MPI

### 📖 Belajar (6 Slide)
- Materi inti dengan gambar hero + narasi karakter **Raka**
- Mini kuis di tiap slide
- Kotak **refleksi kritis** untuk murid menuliskan pendapat

### 🗓️ Kronologi (4 Linimasa)
- Linimasa visual berwarna per periode sejarah
- Komentar Raka yang personal dan kontekstual
- Analisis naratif di panel kanan

### 🎮 Bermain (11 Aktivitas)
| # | Tipe | Topik |
|---|---|---|
| 1 | Jodohkan | Tokoh & Era Kepemimpinan |
| 2 | Urutkan | Kronologi Mei 1998 |
| 3 | Sambung Kalimat | Pilar Kekuasaan Orde Baru |
| 4 | **🔍 Analisis Dokumen HOTS** | Supersemar — Sumber Primer |
| 5 | Klik Objek | Tokoh Tragedi Trisakti |
| 6 | Sambung Kalimat | Capaian Reformasi |
| 7 | Urutkan | Presiden Era Reformasi |
| 8 | Jodohkan | Konsep & Definisi Kunci |
| 9 | Kumpul Objek | Tuntutan Reformasi 1998 |
| 10 | Sambung Kalimat | Fakta Tragedi & Kronologi |
| 11 | Urutkan | Amandemen UUD 1945 |

### ✏️ Berlatih (10 Soal)
- PG (Pilihan Ganda)
- Benar/Salah
- Drag & Drop kata
- PG Kompleks (pilih 2)
- Menjodohkan
- Hasil akhir dengan **sertifikat predikat** (A–E)

---

## 💡 Tips Penggunaan Offline

1. **Simpan semua file dalam satu folder** — jangan pisahkan `index.html` dari folder `asset/`
2. **Buka dengan browser modern** — Chrome, Edge, atau Firefox terbaru
3. **Layar optimal** — 1280×720 px atau lebih besar (akan menyesuaikan otomatis)
4. **Tidak perlu internet** — 100% offline setelah disalin ke komputer/flashdisk

---

## 📐 Spesifikasi Teknis

- **Resolusi stage:** 1280 × 720 px (auto-scale)
- **Format:** Single HTML file (tidak butuh server)
- **Dependensi:** Tidak ada (pure HTML/CSS/JS)
- **Browser support:** Chrome 80+, Edge 80+, Firefox 75+, Safari 14+
- **Ukuran file:** ~100 KB (tanpa aset gambar/audio)

---

*Dikembangkan untuk mendukung pembelajaran Sejarah Fase F Kurikulum Merdeka*  
*MPI ini bersifat offline-first dan dapat didistribusikan melalui flashdisk atau LAN sekolah*
