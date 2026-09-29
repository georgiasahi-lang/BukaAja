# 💌 Interactive Romantic Proposal Website

## 📁 Struktur File

```
proposal/
├── index.html          ← Website utama (semua CSS + JS sudah di dalam)
├── video/
│   └── proposal.mp4   ← 📝 TARUH VIDEO KAMU DI SINI
└── README.md
```

---

## 🎬 Setup Video

1. Siapkan video kamu, format **MP4 (H.264)**
2. Rename jadi **`proposal.mp4`**
3. Taruh di folder **`video/`**
4. Ukuran ideal: **rasio 1:1 (square)**, resolusi min 720×720px
5. Durasi: bebas — progress bar otomatis ngikutin

> Kalau mau ganti nama file, edit baris ini di `index.html`:
> ```html
> <source src="video/proposal.mp4" type="video/mp4"/>
> ```

---

## 🚀 Deploy ke Vercel via GitHub

### Step 1 — Push ke GitHub
```bash
git init
git add .
git commit -m "init: proposal website"
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main
```

### Step 2 — Connect ke Vercel
1. Buka https://vercel.com → **Add New Project**
2. Import repo GitHub kamu
3. Framework: **Other** (static)
4. Build command: *(kosongkan)*
5. Output directory: *(kosongkan / titik `.`)*
6. Klik **Deploy**

### Step 3 — Done! 🎉
Vercel otomatis kasih URL seperti:
`https://nama-project.vercel.app`

---

## 🔧 Kustomisasi

| Yang mau diganti | Lokasi di index.html |
|-----------------|----------------------|
| Nama (MAR) | Cari `MAR,` di `id="lp5"` |
| Isi surat | Cari `id="lp0"` sampai `id="lp5"` |
| Teks ending | Cari `endMain`, `endTitle`, `endSub` |
| Video | `video/proposal.mp4` |
| Teks tombol YES/NO | Cari `btn-yes` dan `btn-no` |
| Dialog NO kabur | Array `noDialogs` di JS |

---

## 📱 Tested Viewport
- 360×800 (Android kelas menengah)
- 390×844 (iPhone 14)
- 412×915 (Pixel 7)
