# KPI Dashboard — PT. Rantai Mulia Kencana 2026

Dashboard laporan KPI Inventory, Warehouse, dan Marketing berbasis web — siap deploy ke Vercel.

## 📦 Isi File

```
kpi-dashboard/
├── index.html     ← Dashboard utama (satu file, zero dependency lokal)
├── vercel.json    ← Konfigurasi Vercel
└── README.md
```

## 🚀 Deploy ke Vercel

### Cara 1 — Vercel CLI (Direkomendasikan)

```bash
# Install Vercel CLI (jika belum)
npm install -g vercel

# Masuk ke folder project
cd kpi-dashboard

# Login ke Vercel
vercel login

# Deploy (ikuti instruksi di terminal)
vercel

# Deploy ke production
vercel --prod
```

### Cara 2 — Vercel Dashboard (Drag & Drop)

1. Buka [vercel.com](https://vercel.com) → Login
2. Klik **"Add New Project"**
3. Pilih **"Upload"** atau drag folder `kpi-dashboard`
4. Klik **Deploy**
5. Selesai! URL otomatis tersedia

### Cara 3 — GitHub Integration

1. Upload folder ke GitHub repo
2. Di Vercel: **Import Git Repository**
3. Pilih repo → Deploy otomatis setiap push

## 📊 Fitur Dashboard

| Tab | Konten |
|-----|--------|
| **Overview** | KPI utama, trend GI vs GR, ITO Ratio, distribusi item |
| **Inventory & SOH** | Nilai stok, klasifikasi fast/slow/dead, top 10 item terbanyak |
| **Good Issue & GR** | Nilai & volume pergerakan barang per bulan, net flow |
| **Work Order** | % pencapaian target WO ≤ 4 hari, gauge per bulan, WO closed |
| **Top Items** | 10 item dengan nilai GI tertinggi Jan–Jun 2026 |

## 📅 Data

- **Periode**: Januari – Juni 2026
- **Perusahaan**: PT. Rantai Mulia Kencana (RMK)
- **Sumber**: Dashboard_Inventory_Warehouse_Marketing_HO_2026.xlsx

## 🛠 Teknologi

- **HTML/CSS/JS** murni — tidak perlu build tool
- **Chart.js v4** — dimuat dari CDN
- **Google Fonts (Inter + DM Mono)** — dimuat dari CDN
- Zero dependency lokal, zero build step
