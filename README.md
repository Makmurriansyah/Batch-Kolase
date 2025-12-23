
<img width="1261" height="779" alt="image" src="https://github.com/user-attachments/assets/a09b9da0-7e94-4cdf-b88c-5d27ef6e9c43" />

# 📸 Batch Auto-Collage Pro

[![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)](https://reactjs.org/)
[![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Gemini AI](https://img.shields.io/badge/Gemini%20AI-121013?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev/)

**Batch Auto-Collage Pro** adalah aplikasi berbasis web modern untuk membuat kolase foto dalam jumlah banyak secara otomatis dan instan. Dirancang untuk kecepatan, privasi, dan kualitas gambar yang tinggi tanpa perlu mengunggah foto Anda ke server.

---

## ✨ Fitur Unggulan

- **🚀 Batch Processing:** Unggah puluhan foto sekaligus dan aplikasi akan otomatis membaginya menjadi beberapa lembar kolase sesuai keinginan Anda (2, 4, 6, atau 9 foto per kolase).
- **🤖 AI Theme Analysis:** Menggunakan **Google Gemini AI** untuk menganalisis koleksi foto Anda dan menyarankan judul serta tema yang sesuai (Opsional).
- **🎨 Color Fidelity & High Quality:** Algoritma rendering Canvas yang dioptimalkan untuk menjaga akurasi warna (sRGB) dan ketajaman gambar asli.
- **🛠️ Manual Editor:**
  - **Pan & Crop:** Geser isi foto di dalam frame untuk komposisi terbaik.
  - **Smart Swap:** Tukar posisi antar foto dengan fitur *Drag & Drop*.
  - **Rotation:** Putar foto yang miring langsung di aplikasi.
- **📥 Download Fleksibel:** Simpan hasil sebagai file **PNG kualitas tinggi** satu per satu atau unduh semua sekaligus dalam satu file **ZIP**.
- **🔒 Privacy First:** Semua pemrosesan foto dilakukan di sisi klien (browser Anda). Foto Anda tidak pernah menyentuh server manapun.
- **📱 Responsive UI:** Tampilan modern dan bersih menggunakan font *Plus Jakarta Sans* yang nyaman di mata.

---

## 🛠️ Teknologi yang Digunakan

- **Frontend:** React 19 & TypeScript
- **Bundler:** Vite
- **Styling:** Tailwind CSS
- **AI Engine:** @google/genai (Gemini 2.0 Flash)
- **Utilities:** JSZip (untuk fitur unduh ZIP), Canvas API (untuk rendering gambar)

---

## 🚀 Cara Penggunaan

### 1. Persiapan Lokal
Pastikan Anda sudah menginstal [Node.js](https://nodejs.org/).

```bash
# Clone repositori ini
git clone https://github.com/username/batch-collage-pro.git

# Masuk ke folder proyek
cd batch-collage-pro

# Instal dependensi
npm install

# Jalankan aplikasi (Development)
npm run dev
```

### 2. Konfigurasi API Key (Opsional)
Untuk mengaktifkan fitur analisis tema otomatis oleh AI, buat file `.env` di root folder:
```env
VITE_GEMINI_API_KEY=isi_dengan_api_key_anda
```
*Dapatkan API Key gratis di [Google AI Studio](https://aistudio.google.com/).*

### 3. Build untuk Produksi
```bash
npm run build
```

---

## ☁️ Cara Deploy (Vercel)

Aplikasi ini sangat mudah dideploy ke Vercel:
1. Hubungkan repositori GitHub Anda ke Vercel.
2. Tambahkan **Environment Variable** jika menggunakan AI:
   - Key: `API_KEY`
   - Value: `[API_KEY_ANDA]`
3. Klik **Deploy**. Selesai!

---

## 💡 Tips Akurasi Warna
Jika Anda mendapati warna gambar berubah saat diunduh, pastikan Anda menggunakan versi terbaru aplikasi ini yang telah menggunakan profil warna `sRGB` eksplisit pada Canvas API dan telah menghapus parameter kompresi non-standar pada ekspor PNG.

---

## 📄 Lisensi
Distribusi di bawah lisensi MIT. Lihat `LICENSE` untuk informasi lebih lanjut.
