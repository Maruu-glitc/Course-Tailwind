# 🚀 Modern Web Layouting with Tailwind CSS

Selamat datang di repositori **catatan belajar Modern UI/UX Development**.  
Tempat ini merangkum **fundamental hingga teknik lanjutan** untuk membangun layout website yang **responsif, rapi, dan estetik** menggunakan **Tailwind CSS**.

---

## 📚 Daftar Isi
- [Flexbox (Satu Dimensi)](#-flexbox-satu-dimensi)
- [CSS Grid (Dua Dimensi)](#-css-grid-dua-dimensi)
- [Mobile First & Breakpoints](#-mobile-first--breakpoints)
- [Glassmorphism (Efek Kaca Modern)](#-glassmorphism-efek-kaca-modern)
- [Contoh: Dashboard Glass UI](#-contoh-dashboard-glass-ui)
- [Link Materi di Repository](#-link-materi-di-repository)

---

## 🧩 Flexbox (Satu Dimensi)
Flexbox digunakan untuk mengatur penempatan elemen **secara fleksibel dalam satu arah**.

### Konsep Utama
- **Parent (Container)**: aktifkan `flex`
- **Main Axis (utama)**: arah default **horizontal**
  - Diatur dengan `justify-*`
- **Cross Axis (tegak lurus)**: arah vertikal
  - Diatur dengan `items-*`

### Properti yang sering dipakai
- `flex-row` / `flex-col`  
  Menentukan arah alur item (samping atau bawah).
- `justify-between`  
  Memberi ruang maksimal antar item.
- `items-center`  
  Menengahkan item secara vertikal.
- `gap-*`  
  Memberi jarak antar item tanpa perlu `margin` manual.

---

## 🏗️ CSS Grid (Dua Dimensi)
CSS Grid dipakai untuk membangun struktur layout yang lebih besar dan kompleks, karena mengatur **baris dan kolom sekaligus**.

### Aturan Utama
- **Grid Columns**: tentukan jumlah kolom di parent, misalnya `grid-cols-3`
- **Spanning (melebar)**: satu item bisa memakan beberapa kolom  
  Gunakan `col-span-*` pada elemen child.
- **Start Position**: menentukan posisi mulai item  
  Gunakan `col-start-*`.

### Strategi Kombinasi
> **Grid** untuk kerangka layout besar, **Flexbox** untuk menata komponen di dalamnya.

---

## 📱 Mobile First & Breakpoints
Tailwind menerapkan pendekatan **mobile-first**:
- Default style = untuk **HP**
- Style untuk layar lebih besar pakai prefix breakpoint

### Breakpoint yang umum
- `md:` → Medium (>= 768px)
- `lg:` → Large (>= 1024px)

### Contoh
`grid-cols-1 md:grid-cols-3`  
Artinya:
- **HP**: 1 kolom
- **Laptop/Tablet (md)**: otomatis menjadi 3 kolom

---

## 🧊 Glassmorphism (Efek Kaca Modern)
Glassmorphism memberi tampilan **frosted glass** yang elegan melalui transparansi dan efek blur.

### Resep Glassmorphism Sempurna
- **Translucency**: `bg-white/20`
- **Backdrop Blur**: `backdrop-blur-md`
- **Border Highlight**: `border border-white/30`
- **Shadow**: `shadow-xl`

> Biasanya efek ini terasa lebih “hidup” saat dipadukan dengan warna background yang kontras.

---

## 🎨🛠️ Contoh: Dashboard Glass UI

Gunakan struktur berikut untuk membuat kartu statistik yang modern:

```html
<!-- Container Grid Responsif -->
<div class="grid grid-cols-1 md:grid-cols-3 gap-6">

  <!-- Card dengan Gaya Sky Glassmorphism -->
  <div class="p-6 rounded-3xl bg-sky-400/20 backdrop-blur-xl border-t border-l border-white/40 border-r border-b border-white/10 shadow-2xl">
    <div class="flex justify-between items-center">
      <div>
        <p class="text-sky-900/70 text-sm font-semibold">Total Visitors</p>
        <h2 class="text-3xl font-bold text-sky-950">1,284</h2>
      </div>
      <div class="p-3 bg-white/30 rounded-2xl">
        <!-- Icon Here -->
      </div>
    </div>
  </div>

</div>
```

---

## 🔗 Link Materi di Repository
- [fundamental-flex.md](fundamental-flex.md)
- [fundamental-grid.md](fundamental-grid.md)
- [fundamental-galassmorphism.md](fundamental-galassmorphism.md)
- Folder latihan:
  - [glassmorphism/](glassmorphism/)
  - [flex-box/](flex-box/)
  - [grid/](grid/)
  - [latihan-gridxflex/](latihan-gridxflex/)

---

### ✨ Catatan
Kalau kamu ingin, next step bisa dibuat versi **README yang lebih lengkap** (misalnya menambahkan screenshot kecil, daftar contoh file per topik, dan “cheat sheet” class Tailwind yang paling sering dipakai).
