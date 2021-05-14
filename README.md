# Template LaTeX Buku Laporan Kerja Praktik ITS

[![latest version](https://img.shields.io/github/v/release/b201lab/template-buku-kp-its)](https://github.com/b201lab/template-buku-kp-its/releases/)
[![commits since latest version](https://img.shields.io/github/commits-since/b201lab/template-buku-kp-its/latest)](https://github.com/b201lab/template-buku-kp-its/commits/master)
[![repo size](https://img.shields.io/github/repo-size/b201lab/template-buku-kp-its)](https://github.com/b201lab/template-buku-ta-its)
[![license](https://img.shields.io/github/license/b201lab/template-buku-kp-its)](./LICENSE)
[![build and test status](https://img.shields.io/github/workflow/status/b201lab/template-buku-kp-its/Build%20LaTeX%20Document)](https://github.com/b201lab/template-buku-kp-its/actions)

Repositori ini berisi template [LaTeX](https://www.latex-project.org/) dari buku laporan kerja praktik yang disesuaikan dengan format yang diberlakukan oleh [Institut Teknologi Sepuluh Nopember](https://www.its.ac.id/) (ITS).
Template ini terinspirasi dari repositori [rohwid/id-thesis-book-min-electics-its](https://github.com/rohwid/id-thesis-book-min-electics-its) dengan perubahan yang menyesuaikan kebutuhan pembukuan laporan kerja praktik ITS serta dengan pemangkasan isi.
Template yang dibuat saat ini baru mengikuti aturan yang diberlakukan oleh [Departemen Teknik Komputer](https://www.its.ac.id/komputer/) FTEIC - ITS dengan sedikit penyesuaian, sehingga, secara penuh template ini belum mewakili aturan yang berlaku secara umum di setiap departemen yang ada di ITS.

> Perlu diketahui, template ini bukanlah template resmi yang dikeluarkan oleh ITS maupun departemen-departemen yang ada di bawah naungan ITS.

## Fitur

- Format ukuran halaman, margin, dan font yang disesuaikan dengan aturan yang berlaku di ITS.
- Disertai halaman-halaman yang diperlukan seperti sampul, lembar pengesahan, kata pengantar, dsb.
- Pembuatan daftar isi, daftar gambar, daftar tabel, dan daftar pustaka secara otomatis.
- Penomoran halaman, gambar, tabel, dan referensi secara otomatis.
- Penambahan gambar dengan format JPEG, PNG, maupun format lain pada dokumen.
- Penambahan persamaan ilmiah, tabel, dan kode program pada dokumen.
- Kompilasi dokumen secara otomatis menggunakan [GitHub Actions](https://github.com/features/actions).

## Cara Menggunakan Template

Bagian utama dokumen terletak pada file [`main.tex`](./main.tex) yang digunakan untuk mengatur package LaTeX yang digunakan serta file lain yang akan diinputkan pada dokumen.
Setelah kompilasi dilakukan, hasilnya akan ada beberapa file `main` dengan format yang berbeda.
Yang paling utama adalah file `main.pdf` yang merupakan hasil akhir dari proses kompilasi dokumen.

Selain file `main.tex`, ada juga beberapa bagian lain dari template ini yang bisa diubah, seperti:
- **[`bab`](./bab)**, berisi file `*.tex` dari setiap bab yang akan dimasukkan pada buku laporan kerja praktik.
- **[`pengesahan`](./pengesahan)**, berisi file `*.tex` dari lembar pengesahan untuk buku laporan kerja praktik.
- **[`sampul`](./sampul)**, berisi file `*.tex` dari sampul luar dan dalam untuk buku laporan kerja praktik.
- **[`lainnya`](./lainnya)**, berisi file `*.tex` dari halaman lain yang akan dimasukkan pada buku laporan kerja praktik.
- **[`gambar`](./gambar)**, berisi file `*.jpg`, `*.png`, maupun format gambar lain yang akan dimasukkan pada dokumen.
- **[`tabel`](./tabel)**, berisi file `*.tex` dari tabel yang akan dimasukkan pada dokumen.
- **[`program`](./program)**, berisi file kode program yang akan dimasukkan pada dokumen.
- **[`pustaka/pustaka.bib`](./pustaka/pustaka.bib)**, berisi daftar referensi yang akan dimasukkan pada dokumen.

> Penjelasan lebih lanjut mengenai penggunaan template ini akan dijelaskan dengan comment yang tersedia pada setiap file yang ada.

## Contoh Penggunaan Template

Berikut adalah daftar repositori lain yang menggunakan template yang berasal dari repositori ini:
- [threeal/buku-kp-ati-warehouse](https://github.com/threeal/buku-kp-ati-warehouse).

## Lisensi

Kode sumber yang ada di repositori ini dilisensikan di bawah [lisensi MIT](./LICENSE).
