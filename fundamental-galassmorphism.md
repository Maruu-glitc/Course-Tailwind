# Fundamental Glassmorphism

## Empat Pilar Utama Glassmorphism

Untuk mendapatkan efek kaca (glassmorphism) yang sempurna, kamu wajib mengombinasikan 4 elemen ini:

1. **Transparansi Latar (Translucency)**  
   Gunakan warna latar belakang dengan opasitas rendah.  
   Contoh kelas:
   - `bg-white/30`
   - `bg-black/20`

2. **Efek Buram Belakang (Backdrop Blur)**  
   Menyamarkan objek yang ada di belakang elemen.  
   Contoh kelas:
   - `backdrop-blur-md`
   - `backdrop-blur-lg`

3. **Garis Tepi Tipis (Subtle Border)**  
   Memberikan kesan potongan kaca yang tajam.  
   Contoh kelas:
   - `border border-white/20`

4. **Bayangan Halus (Soft Shadow)**  
   Memberikan efek kedalaman agar elemen terlihat melayang.  
   Contoh kelas:
   - `shadow-xl`

---

## Mengenal Backdrop Blur

Ini adalah **nyawa** dari glassmorphism. Perintah ini tidak memburamkan konten di dalam kotak, tapi memburamkan apa pun yang ada di belakang kotak tersebut.

Contoh variasi:
- `backdrop-blur-sm`: efek kaca tipis
- `backdrop-blur-md`: efek kaca standar
- `backdrop-blur-xl`: efek kaca sangat tebal/sangat buram

---

## Aturan Penggunaan

Agar efek kaca terlihat nyata, perhatikan aturan ini:

- **Latar Belakang Berwarna**  
  Efek ini wajib diletakkan di atas background yang berwarna, gradien, atau gambar.  
  Jika background-nya putih polos, efek kaca tidak akan terlihat.

- **Warna Teks**  
  Gunakan warna teks yang kontras (`white` atau abu-abu gelap) agar tetap mudah dibaca di atas kaca yang transparan.
