# Daftar Produk Toko (JavaFX)

Aplikasi desktop sederhana untuk mencatat produk toko, dibuat dengan JavaFX
sebagai tugas individu mata kuliah Pemrograman Lanjut. Strukturnya mengikuti
pola praktikum: `MainApp`, `Navigator`, controller, model, data, dan FXML.

Nama / NIM: Gregorius Putra Chrisaty Antonio / 2521421

## Fitur

- Menambah produk lewat form (kode, nama, kategori Makanan/Minuman, harga)
- Tabel produk (kode, nama, kategori, harga)
- Pencarian berdasarkan nama produk lewat tombol **Cari** (tombol **Reset** menampilkan semua)
- Tombol **Lihat Detail** membuka halaman detail produk yang dipilih
- Validasi: nama tidak boleh kosong, harga harus angka lebih dari nol
- Data disimpan selama aplikasi berjalan (tanpa database)

## Kebutuhan

- JDK 17
- Maven
- JavaFX 21 (diunduh otomatis oleh Maven lewat `pom.xml`)

## Cara menjalankan

### Lewat terminal

1. Clone repositori:
   ```
   git clone https://github.com/gregorius06/daftar-produk-toko-javafx.git
cd daftar-produk-toko-javafx
   ```
2. Jalankan aplikasi:
   ```
   mvn javafx:run
   ```

### Lewat NetBeans

1. Buka **File > Open Project**, lalu pilih folder proyek ini.
2. Klik kanan proyek > **Run Maven > Goals...**
3. Isi `javafx:run`, lalu klik **OK**.

## Struktur proyek

```
src/main/java/kelas
├── MainApp.java
├── Navigator.java
├── controller   (FormController, DaftarController, DetailController)
├── data         (DataProduk)
└── model        (Produk)

src/main/resources/kelas
├── form.fxml
├── daftar.fxml
├── detail.fxml
└── styles/app.css
```

## Tampilan aplikasi

### Form tambah produk
![Form tambah produk](screenshots/form.png)

### Daftar produk
![Daftar produk](screenshots/daftar.png)

### Hasil pencarian
![Hasil pencarian](screenshots/cari.png)

### Detail produk
![Detail produk](screenshots/detail.png)

### Validasi input
![Validasi input](screenshots/validasi.png)
