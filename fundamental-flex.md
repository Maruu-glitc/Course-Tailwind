# 📌 Fundamental Flexbox (Tailwind CSS)

Flexbox adalah sistem layout satu dimensi yang sangat kuat untuk mengatur posisi elemen (*items*) di dalam sebuah container.

---

## 1) Konsep Utama: Parent & Child

Dalam Flexbox, ada perbedaan aturan antara container (*parent*) dan elemen yang berada langsung di dalamnya (*children*):

- **Flex Container (Parent)**: elemen tempat kamu memberikan class **`flex`**
- **Flex Items (Children)**: elemen-elemen yang berada langsung di bawah container tersebut

---

## 2) Arah Sumbu (Flex Direction)

Secara default, Flexbox akan menyusun item secara horizontal:

- **`flex-row`**: item berjejer ke samping *(default)*
- **`flex-col`**: item berderet ke bawah *(seperti tumpukan)*

---

## 3) Penyelarasan (Alignment)

### A. Main Axis (Sumbu Utama) — `justify-*`

Digunakan untuk mengatur jarak antar item pada **sumbu utama**.  
(berjalan horizontal jika **`flex-row`**, vertikal jika **`flex-col`**)

- **`justify-start`**: rata kiri / atas
- **`justify-center`**: rata tengah
- **`justify-end`**: rata kanan / bawah
- **`justify-between`**: jarak maksimal, item pertama di ujung dan item terakhir di ujung
- **`justify-around`**: ruang di sekeliling item secara rata

### B. Cross Axis (Sumbu Silang) — `items-*`

Digunakan untuk mengatur posisi item secara tegak lurus terhadap sumbu utama.

- **`items-start`**: rata atas / awal
- **`items-center`**: rata tengah (vertikal)
- **`items-end`**: rata bawah / akhir

---

## 4) Jarak Antar Item (Gap)

Daripada memakai `margin` pada tiap item, gunakan **`gap`** pada container:

- **`gap-4`**: jarak 1rem (16px) di antara semua item
- **`gap-x-2`**: jarak horizontal saja
- **`gap-y-2`**: jarak vertikal saja


🚀 Contoh Latihan (Copy-Paste ke HTML)
Gunakan kode ini di dalam file HTML kamu untuk melihat cara kerjanya:

<!-- Container yang menengahkan kotak di dalamnya -->
<div class="flex justify-center items-center gap-4 bg-gray-200 h-64">
  <div class="p-10 bg-blue-500 text-white">Kotak 1</div>
  <div class="p-10 bg-red-500 text-white">Kotak 2</div>
  <div class="p-10 bg-green-500 text-white">Kotak 3</div>
</div>

