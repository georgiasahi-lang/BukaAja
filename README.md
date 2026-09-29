# 💌 Interactive Romantic Proposal Website

## 📁 Struktur File

```
proposal/
├── index.html           ← Website utama
├── audio/
│   └── bgm.mp3         ← 📝 TARUH MUSIK BGM DI SINI
├── video/
│   └── proposal.mp4    ← 📝 TARUH VIDEO DI SINI
└── README.md
```

---

## 🎵 Setup Musik (BGM)

1. Siapkan file musik format **MP3**
2. Rename jadi **`bgm.mp3`**
3. Taruh di folder **`audio/`**
4. Musik akan **loop otomatis** dari scene envelope
5. Saat user klik **YES** → musik **fade out** pelan lalu mati

> Rekomendasi: lagu piano instrumental / acoustic romantic

---

## 🎬 Setup Video

1. Siapkan video format **MP4 (H.264)**
2. Rename jadi **`proposal.mp4`**
3. Taruh di folder **`video/`**
4. Rasio ideal: **1:1 (square)**, min 720×720px
5. Video **tidak loop** — setelah selesai otomatis lanjut ke ending

---

## 🚀 Deploy ke Vercel via GitHub

```bash
# 1. Push ke GitHub
git init
git add .
git commit -m "init: proposal website"
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main

# 2. Vercel → Add New Project → import repo
#    Framework: Other (static)
#    Build command: (kosongkan)
#    Output dir: (kosongkan / titik)
#    → Deploy!
```

---

## ✏️ Kustomisasi Cepat

| Yang diganti | Lokasi di index.html |
|---|---|
| Nama (MAR) | Cari `MAR,` di `id="lp3"` |
| Isi surat | `id="lp0"` sampai `id="lp3"` |
| Teks ending | `endSo`, `endMain`, `endTitle`, `endSub` |
| Dialog NO kabur | Array `noDialogs` di JS |
| Quote di video | `.vbq-quote` di HTML |
| Volume BGM | `bgm.volume = 0.5` di JS (0.0–1.0) |

---

## 🔧 Changelog Update

- ✅ Dialog NO sekarang popup dari atas (tidak menimpa teks)
- ✅ BGM mp3 loop, mati saat YES diklik (fade out)
- ✅ Isi surat diperbarui sesuai permintaan
- ✅ Video scene ada teks quote di atas & bawah (tidak polos)
- ✅ Bug video loop → sekarang fixed, lanjut ke ending
