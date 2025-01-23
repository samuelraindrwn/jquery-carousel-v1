## 📋 Deskripsi

Kode ini adalah implementasi carousel responsif yang mendukung fitur auto-looping, pause on hover, navigasi tombol, serta bullet pagination. Carousel ini dirancang fleksibel dengan kemampuan penyesuaian melalui konfigurasi responsif untuk berbagai ukuran layar. Sangat cocok untuk ditambahkan ke proyek web modern.

## ✨ Fitur Utama

- **Responsif**: Carousel menyesuaikan jumlah item yang ditampilkan berdasarkan lebar layar.
- **Auto-looping**: Carousel dapat bergerak otomatis dengan interval waktu tertentu.
- **Pause on Hover**: Auto-loop akan berhenti sementara saat pengguna mengarahkan kursor ke carousel.
- **Navigasi Manual**: Terdapat tombol navigasi "sebelumnya" dan "berikutnya".
- **Pagination Bullet**: Indikator posisi carousel berupa bullet yang dapat diklik.
- **Dukungan Infinite Scrolling**: Opsi untuk mengaktifkan navigasi tanpa batas.

---

## 🛠️ Cara Menggunakan

### 1. **Tambahkan Markup HTML**
Salin kode HTML berikut ke dalam file proyek Anda:

```html
<div class="carousel">
  <div class="wrapper">
    <div class="item-wrapper">
      <div class="item">Item 1</div>
      <div class="item">Item 2</div>
      <!-- Tambahkan lebih banyak item sesuai kebutuhan -->
    </div>
  </div>
  <div class="controls">
    <button class="control prev"><i class="fas fa-chevron-left"></i></button>
    <div class="bullet-wrapper"></div>
    <button class="control next"><i class="fas fa-chevron-right"></i></button>
  </div>
</div>
```

### 2. **Tambahkan Gaya CSS**
Tambahkan gaya CSS ke dalam file `<style>` atau file CSS eksternal Anda.

### 3. **Tambahkan Library yang Diperlukan**
Masukkan library jQuery dan Font Awesome ke file Anda:

```html
<script src="https://code.jquery.com/jquery-3.6.4.min.js"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
```

### 4. **Konfigurasi JavaScript**
Gunakan fungsi `createCarousel()` yang sudah tersedia untuk menginisialisasi carousel:

```javascript
$(function () {
  createCarousel({
    visibleItems: 4,
    slideBy: 4,
    autoLoop: true,
    loopInterval: 3000,
    responsive: {
      1200: { visibleItems: 4, slideBy: 4, bullet: true },
      992: { visibleItems: 3, slideBy: 3, bullet: true },
      768: { visibleItems: 2, slideBy: 2, bullet: false },
      576: { visibleItems: 1, slideBy: 1, bullet: false },
    },
  });
});
```

---

## 🔧 Konfigurasi

| Opsi               | Default          | Deskripsi                                                                 |
|--------------------|------------------|---------------------------------------------------------------------------|
| `visibleItems`     | `4`              | Jumlah item yang terlihat dalam satu waktu.                              |
| `slideBy`          | `4`              | Jumlah item yang digeser dalam satu klik.                                |
| `itemGap`          | `20`             | Jarak antar item dalam carousel.                                         |
| `bullet`           | `true`           | Mengaktifkan/mematikan pagination bullet.                                |
| `transition`       | `300`            | Durasi transisi (dalam milidetik).                                       |
| `infiniteCarousel` | `false`          | Mengaktifkan navigasi tanpa batas.                                       |
| `autoLoop`         | `false`          | Mengaktifkan pergerakan otomatis.                                        |
| `loopInterval`     | `3000`           | Interval waktu looping otomatis (dalam milidetik).                       |

---

## 🖼️ Tangkapan Layar

Tambahkan tangkapan layar carousel Anda untuk membantu pengguna memahami bagaimana tampilannya.

---

## ⚠️ Catatan

- Pastikan file CSS dan JavaScript di-link dengan benar.
- Gunakan class yang sesuai agar tidak terjadi konflik dengan elemen lain.
- Tes pada berbagai perangkat untuk memastikan kompatibilitas.

---

## 🤝 Kontribusi

Jika Anda memiliki saran atau ingin berkontribusi untuk meningkatkan proyek ini, jangan ragu untuk mengirimkan pull request atau membuka issue.

---

## 📜 Lisensi

Proyek ini menggunakan lisensi MIT. Anda bebas menggunakannya untuk keperluan pribadi maupun komersial. Jangan lupa untuk memberikan kredit! 😄

