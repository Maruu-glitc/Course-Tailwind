# 🏁 Fundamental CSS Grid (Tailwind CSS)

Grid Layout digunakan untuk mengatur tata letak yang lebih kompleks dan terstruktur, seperti **galeri foto**, **dashboard**, atau **layout halaman utama**.

---

## 1) Perbedaan Utama dengan Flexbox

- **Flexbox**: satu dimensi (fokus mengatur **baris** *atau* **kolom**).
- **Grid**: dua dimensi (mengatur **baris** dan **kolom** sekaligus).

---

## 2) Mengaktifkan Grid

Tambahkan class `grid` pada elemen pembungkus/parent (container).

---

## 3) Menentukan Kolom (`grid-cols-*`)

Kamu menentukan berapa kolom yang ingin dibuat:
grid-col mengatur jumlah kolom yang anda inginkan max 12

- `grid-cols-2` → 2 kolom sama besar
- `grid-cols-3` → 3 kolom sama besar
- `grid-cols-12` → standar yang sering dipakai untuk layout kompleks

---

## 4) Mengatur Jarak (Gap)

Gunakan `gap` untuk memberi ruang antar item:

- `gap-4` → jarak rata untuk baris dan kolom
- `gap-x-4` → hanya jarak antar kolom
- `gap-y-4` → hanya jarak antar baris

---

## 5) Menggabungkan Kolom & Baris (Spanning)

Jika satu item perlu memakan lebih dari satu kolom/baris:
colspan mengatur berapa jumlah kolom yang ingin di makan (child) yang tadi sudah di atur oleh (grid-col)

- `col-span-2` → memakan 2 kolom
- `col-span-full` → memakan seluruh lebar kolom
- `row-span-2` → memakan 2 baris

---

## Contoh Singkat

> Misal 3 kolom dengan gap, lalu satu item melebar 2 kolom.

```html
<div class="grid grid-cols-3 gap-4">
  <div class="bg-slate-200 p-4">Item 1</div>
  <div class="bg-slate-200 p-4 col-span-2">Item 2 (lebar 2 kolom)</div>
  <div class="bg-slate-200 p-4">Item 3</div>
</div>
```

---

## Tips Praktis (Opsional)

- Untuk layout responsif, kamu bisa mengatur jumlah kolom per breakpoint, misalnya:
  - `grid-cols-1 sm:grid-cols-2 lg:grid-cols-3`

- Kalau mau tinggi otomatis rapi untuk item card, biasanya dibantu dengan `p-*`, `rounded-*`, dan `bg-*` di masing-masing item.
