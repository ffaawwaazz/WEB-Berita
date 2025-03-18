# WEB-Berita

LINK WEB :  https://ffaawwaazz.github.io/WEB-Berita/

Berikut adalah penjelasan kode HTML, CSS, dan JavaScript dalam file yang telah saya buat. 

---

# Liga Korupsi Indonesia - Berita CNN Indonesia  

## Deskripsi  
Proyek ini adalah halaman web sederhana yang menampilkan daftar berita mengenai korupsi di Indonesia. Pengguna dapat mengklik berita untuk membuka detail berita di tab baru.  

---

## Struktur Kode  

### 1. **HTML** (Struktur Halaman)  
Kode ini menggunakan HTML5 dengan bahasa utama **Indonesia** (`lang="id"`). Struktur utama halaman terdiri dari:  

- **Header**:  
  - Memuat logo **CNN Indonesia** dan menu navigasi dengan beberapa kategori berita seperti **Home, Ekonomi, Olahraga, Teknologi, Hiburan**.  

- **Main Content**:  
  - Memuat judul utama **LIGA KORUPSI INDONESIA**.  
  - Daftar berita disusun dalam **container** dengan setiap berita berbentuk **kotak (div class="news-item")** yang berisi **gambar, judul berita, dan waktu publikasi**.  
  - Setiap berita memiliki fungsi **onclick**, yang memanggil JavaScript untuk membuka halaman baru dengan konten berita.  

- **Footer**:  
  - Menampilkan hak cipta **CNN Indonesia 2025**.  

---

### 2. **CSS** (Gaya dan Tampilan)  
CSS digunakan untuk mengatur tata letak dan tampilan website:  

- **`body`** → Menggunakan font Arial, warna latar belakang abu-abu (`#f4f4f4`).  
- **`top-bar`** → Header berwarna merah (`#cc0000`) dengan teks putih.  
- **`nav`** → Menu navigasi berbentuk horizontal dengan teks tebal.  
- **`.news-container`** → Berita disusun dalam kolom ke bawah (**align-items: flex-start**).  
- **`.news-item`** → Setiap berita berbentuk **kotak** dengan:  
  - **Gambar** di sisi kiri.  
  - **Judul berita dan waktu publikasi** di sisi kanan.  
  - **Border** abu-abu tebal (`3px solid #807474`).  
  - **Efek shadow** agar terlihat seperti kartu.  
- **`footer`** → Latar belakang merah dengan teks putih.  

---

### 3. **JavaScript** (Interaksi Halaman)  
Fungsi `openNewsPage(title, content)` digunakan untuk membuka tab baru dengan isi berita:  

```js
function openNewsPage(title, content) {
    const newsWindow = window.open("", "_blank"); 
    newsWindow.document.write(`
        <html>
        <head>
            <title>${title}</title>
            <style>
                body { font-family: Arial, sans-serif; padding: 20px; }
                h1 { color: #d32f2f; }
            </style>
        </head>
        <body>
            <h1>${title}</h1>
            <p>${content}</p>
        </body>
        </html>
    `);
}
```

- **window.open("", "_blank")** → Membuka jendela baru.  
- **document.write()** → Menuliskan **judul dan isi berita** ke dalam tab baru.  
- **CSS di dalam JavaScript** → Mengatur font dan warna judul berita.  

---

## Cara Menjalankan  
1. Simpan file sebagai **index.html**.  
2. Simpan logo CNN di **LOGOcnn.png** di folder yang sama.  
3. Simpan gambar berita (LKI01.jpg, LKI02.jpg, dst.) di folder yang sama.  
4. Jalankan file **index.html** di browser.  

---

Dengan penjelasan ini, Anda bisa menaruhnya di **README.md** di GitHub agar lebih mudah dipahami oleh orang lain. 🚀
