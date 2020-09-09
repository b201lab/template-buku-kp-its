# Template Buku Laporan Kerja Praktek ITS (Institut Teknologi Sepuluh Nopember) Berbasis LaTeX

Repositori ini berisi _template_ dari buku laporan kerja praktek berbasis [**LaTeX**](https://www.latex-project.org/) yang disesuaikan dengan format yang diberlakukan oleh **Institut Teknologi Sepuluh Nopember**.
_Template_ ini terinspirasi dari repositori [**rohwid/id-thesis-book-min-electics-its**](https://github.com/rohwid/id-thesis-book-min-electics-its) yang digunakan sebagai _template_ buku tesis **Jaringan Cerdas Multimedia** **FTEIC** - **ITS** dengan perubahan yang menyesuaikan kebutuhan pembukuan laporan kerja praktek serta dengan pemangkasan isi.
_Template_ yang dibuat saat ini baru mengikuti aturan yang diberlakukan oleh **Departemen Teknik Elektro** **FTEIC** - **ITS** dengan sedikit penyesuaian, sehingga, secara penuh _template_ ini belum mewakili aturan yang berlaku secara umum di setiap departemen yang ada di **ITS**.
Untuk itu, diharapkan adanya kontribusi dari pihak yang bersedia membantu agar nantinya _template_ ini bisa konsisten digunakan setiap tahun dengan menyesuaikan aturan dari setiap departemen yang ada di **ITS**.

## Fitur

- Format ukuran halaman, _margin_, dan _font_ yang disesuaikan dengan aturan yang berlaku di **ITS**.
- Sampul yang dibuat otomatis melalui **LaTeX**.
- Penomoran halaman, gambar, tabel, dan _citation_ secara otomatis.
- _Input_ gambar dengan format **JPEG** maupun **PNG**.
- Pembuatan persamaan, tabel, dan _code snippet_.

## Penjelasan Singkat LaTeX

[**TeX**](https://en.wikipedia.org/wiki/TeX) merupakan salah satu sistem _typesetting_ yang digunakan untuk membuat dokumen secara mudah, dengan format yang konsisten.
**LaTeX** sendiri merupakan salah satu turunan dari **TeX** dengan penambahan lebih banyak fitur dan _package_ yang membantu pembuatan dokumen dengan lebih mudah.
**LaTeX** bersamaan dengan **TeX** sendiri ibaratnya merupakan bahasa pemrograman, agar dapat menghasilkan dokumen yang siap dicetak, diperlukan sebuah _compiler_ yang akan menerjemahkan setiap perintah yang ditulis menggunakan bahasa tersebut.
Untuk saat ini ada beberapa _compiler_ yang bisa digunakan untuk meng-_compile_ **LaTeX**, salah satunya adalah [**TeX Live**](https://www.tug.org/texlive/).
**TeX Live** sendiri dipilih karena alasan _cross-platform_, sehingga bisa digunakan pada sistem operasi yang berbeda, terutama **Windows** dan **Linux**.

## Cara Menggunakan LaTeX

- [Instalasi dan penggunaan **TeX Live**](./bantuan/instalasi-tex-live.md).
- [Integrasi template dengan **Visual Studio Code**](./bantuan/integrasi-vs-code.md).
- [_Syntax_ dasar **LaTeX**](./bantuan/syntax-dasar-latex.md).

## Cara Menggunakan Template

Bagian utama dokumen terletak pada _file_ `main.tex` yang digunakan untuk mengatur _package_ apa saja yang digunakan serta _file_ lain yang akan di-_inputkan_.
Setelah dilakukan kompilasi, hasilnya akan ada banyak _file_ `main` dengan format yang berbeda.
Yang terpenting adalah _file_ `main.pdf` yang merupakan hasil akhir dari kompilasi dokumen tersebut.

Selain itu ada beberapa bagian lain dari _template_ ini selain `main.pdf` yang bisa diubah, seperti:
- _Folder_ `bab` yang berisi _file_ `*.tex` dari bab yang akan dimasukkan pada buku laporan kerja praktek.
- _Folder_ `pengesahan` yang berisi _file_ `*.tex` dari lembar pengesahan untuk buku laporan kerja praktek.
- _Folder_ `sampul` yang berisi _file_ `*.tex` dari sampul luar dan dalam untuk buku laporan kerja praktek.
- _Folder_ `lainnya` yang berisi _file_ `*.tex` dari halaman lain yang akan dimasukkan pada buku laporan kerja praktek.
- _Folder_ `gambar` yang berisi _file_ `*.jpg`, `*.png`, maupun format gambar lain yang akan dimasukkan pada dokumen.
- _Folder_ `tabel` yang berisi _file_ `*.text` dari tabel yang akan dimasukkan pada dokumen.
- _Folder_ `program` yang berisi _file_ kode program yang akan dimasukkan pada dokumen.
- _File_ `pustaka/pustaka.bib` yang berisi daftar referensi yang akan dimasukkan pada dokumen.

> Penjelasan lebih lanjut mengenai modifikasi pada template akan dijelaskan dengan _comment_ yang bisa dilihat langsung pada masing masing _file_ yang tersedia.

## Kontribusi

Karena keterbatasan pengetahuan mengenai aturan yang berlaku di setiap departemen di **ITS** serta agar _template_ yang dibuat ini bisa berkembang dengan fitur yang lebih banyak, diharapkan adanya kontribusi dari pihak lain yang bersedia untuk membantu.
Untuk melakukan kontribusi, siapapun bisa memulai dengan melakukan _fork_ pada repositori utama _template_ ini yang ada di [**threeal/template-buku-kp-its**](https://github.com/threeal/template-buku-kp-its), kemudian membuat perubahan dan melakukan _pull request_.
Jika terdapat masalah dari _template_ ini maupun hal yang berkaitan dengan _template_ ini, jangan ragu untuk membuat _issue_ baru pada halaman _issues_ yang bisa diakses [disini](https://github.com/threeal/template-buku-kp-its/issues).