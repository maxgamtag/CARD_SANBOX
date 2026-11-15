# 🃏 KartuSandbox — Meja Kartu Remi Virtual (1–8 Pemain)

Aplikasi web permainan kartu remi berbasis **sandbox** (*open-source*, ringan, dan *zero-dependency* build step) yang memungkinkan **1 hingga 8 pemain** bermain bebas di satu meja virtual—mulai dari **Solitaire (1 pemain)** hingga **Tepok Nyamuk, Cangkulan, Capsa, dan Remi (2–8 pemain)**.

---

## ✨ Fitur Utama

- **3 Mode Bermain Fleksibel**:
  - **Mode Solo (1 Pemain)**: Langsung masuk meja tanpa koneksi untuk Solitaire atau eksperimen susunan kartu.
  - **Mode WiFi / P2P Lokal (`Host = Server`)**: Menggunakan **WebRTC (`PeerJS`)** di mana perangkat pembuat room otomatis menjadi *server* lokal. Pergerakan kartu dikirim langsung antarperangkat (*peer-to-peer*) dengan latensi sangat rendah.
  - **Mode Cloud Room (Opsional)**: Mendukung sinkronisasi berbasis Firebase Firestore untuk permainan jarak jauh.
- **Kustomisasi Deck & Joker**:
  - Atur **1 hingga 10 deck** standar (52–520 kartu) dan **0 hingga 30 kartu Joker** secara langsung.
- **Fitur Pengacak Kartu & Kontrol Meja**:
  - **Kocok Deck (`🔀`)**: Mengacak urutan seluruh kartu di tumpukan utama.
  - **Tarik Acak (`🎲`)**: Mengambil 1 kartu secara acak dari deck langsung masuk ke tangan pribadi.
  - **Sebar Acak (`✨`)**: Menyebar kartu dari deck ke area tengah meja dengan koordinat dan rotasi acak.
  - **Bagi Kartu (`🃏`) & Kumpulkan (`📥`)**: Membagi kartu per pemain atau membagi rata seluruh sisa deck, serta mengumpulkan kembali semua kartu ke deck.
- **Tangan Pribadi (*Private Hand*) & Meja Publik (*Public Table*)**:
  - Kartu di area bawah layar hanya terlihat oleh pemiliknya, sementara pemain lain hanya melihat jumlah kartu di kursi masing-masing.
  - Mendukung geser (*drag & drop*) maupun sentuhan layar (*touch*) di HP dan desktop.

---

## 🚀 Cara Publikasi ke GitHub & GitHub Pages

Karena seluruh aplikasi dikemas dalam **satu file `index.html`** tanpa proses *build* yang rumit, proyek ini bisa langsung di-hosting secara gratis di **GitHub Pages**:

1. **Buat Repository Baru di GitHub**
   - Masuk ke [GitHub](https://github.com/new), beri nama repository (misalnya `kartu-sandbox`), dan pilih **Public**.
2. **Upload File**
   - Unggah `index.html` dan `README.md` ke branch `main`.
3. **Aktifkan GitHub Pages**
   - Buka tab **Settings → Pages** pada repository Anda.
   - Pada bagian **Build and deployment → Source**, pilih **Deploy from a branch**.
   - Pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.
   - Dalam ±1 menit, aplikasi dapat diakses publik melalui `https://<username-anda>.github.io/kartu-sandbox/` dan langsung siap dimainkan lewat **Mode Solo** maupun **Mode WiFi / P2P Lokal**.

---

## 📄 Lisensi (Open Source — MIT License)

```text
MIT License

Copyright (c) 2026 KartuSandbox Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```