Berikut adalah versi **Markdown lengkap** yang langsung bisa disalin ke file `README.md` atau posting GitHub:


# 📡 Menjalankan Datagram Node CLI di VPS (24 Jam Non-Stop)

Panduan ini menjelaskan cara menjalankan node **Datagram** di server VPS Anda agar mendapatkan poin setiap 24 jam tanpa henti.

---

## 🔗 LANGKAH 1: Daftar dan Dapatkan API Key

1. Buka link berikut:  
   👉 [https://dashboard.datagram.network?ref=116831363](https://dashboard.datagram.network?ref=116831363)
2. Daftarkan akun menggunakan email Anda.
3. Login ke akun Anda dan buka **Dashboard**.
4. Navigasikan ke **Wallet > Licence**.
5. Buat lisensi baru, lalu **copy API Key** yang muncul.


## 💻 LANGKAH 2: Siapkan VPS Anda

Gunakan aplikasi **Termius** (tersedia di Windows & Android) atau terminal lain untuk akses SSH ke VPS.

> Jika belum memiliki VPS, Anda bisa membelinya lewat Shopee atau penyedia VPS lainnya.

### 🛠️ Jalankan perintah berikut di VPS:

Berikut adalah versi **blok kode per langkah**, dipisah dan rapi agar bisa langsung disalin satu per satu:

---

### 1. Buat folder `datagram` dan masuk ke dalamnya:

```bash
mkdir datagram
cd datagram
```

---

### 2. Unduh binary Datagram CLI (Linux 64-bit):

```bash
wget -O datagram-cli https://github.com/Datagram-Group/datagram-cli-release/releases/latest/download/datagram-cli-x86_64-linux
```

---

### 3. Jadikan file bisa dieksekusi:

```bash
chmod +x datagram-cli
```



## 🚀 LANGKAH 3: Jalankan Node Datagram

### 1. Buat screen baru agar node tetap berjalan meskipun Anda keluar:

```bash
screen -S datagram
```

### 2. Jalankan CLI dengan API key Anda:

```bash
./datagram-cli run -- -key YOUR_API_KEY
```

> Ganti `YOUR_API_KEY` dengan API Key Anda yang didapatkan dari Dashboard.

---

## 📥 Tips & Perintah Tambahan

* **Keluar dari screen tanpa mematikan node:**

  ```
  Ctrl + A lalu tekan D
  ```

* **Masuk kembali ke screen:**

  ```bash
  screen -r datagram
  ```

---

## 💬 FAQ

**Q: Apakah saya harus membuka VPS terus-menerus?**
A: Tidak perlu. Dengan screen, node tetap berjalan meskipun Anda logout dari VPS.

**Q: Apakah ini gratis?**
A: Menjalankan node gratis, namun Anda perlu menyediakan VPS (berbayar atau trial).

---

## 🤝 Referral & Dukungan

Gunakan link referral ini saat mendaftar:
👉 [https://dashboard.datagram.network?ref=116831363](https://dashboard.datagram.network?ref=116831363)

---

Jika mengalami kendala hubungi Whatsapp https://wa.me/6282363630185
---


