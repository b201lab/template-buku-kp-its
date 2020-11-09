# Template Buku Laporan Kerja Praktik ITS (Institut Teknologi Sepuluh Nopember) Berbasis LaTeX

Repositori ini berisi _template_ dari buku laporan kerja praktik berbasis [**LaTeX**](https://www.latex-project.org/) yang disesuaikan dengan format yang diberlakukan oleh **Institut Teknologi Sepuluh Nopember**.
_Template_ ini terinspirasi dari repositori [**rohwid/id-thesis-book-min-electics-its**](https://github.com/rohwid/id-thesis-book-min-electics-its) yang digunakan sebagai _template_ buku tesis **Jaringan Cerdas Multimedia** **FTEIC** - **ITS** dengan perubahan yang menyesuaikan kebutuhan pembukuan laporan kerja praktik serta dengan pemangkasan isi.
_Template_ yang dibuat saat ini baru mengikuti aturan yang diberlakukan oleh **Departemen Teknik Elektro** **FTEIC** - **ITS** dengan sedikit penyesuaian, sehingga, secara penuh _template_ ini belum mewakili aturan yang berlaku secara umum di setiap departemen yang ada di **ITS**.
Untuk itu, diharapkan adanya kontribusi dari pihak yang bersedia membantu agar nantinya _template_ ini bisa konsisten digunakan setiap tahun dengan menyesuaikan aturan dari setiap departemen yang ada di **ITS**.

> Perlu diketahui, _template_ ini bukanlah _template_ resmi yang dikeluarkan oleh **ITS** maupun departemen-departemen yang ada di bawah naungan **ITS**.

## Fitur

- Format ukuran halaman, _margin_, dan _font_ yang disesuaikan dengan aturan yang berlaku di **ITS**.
- Disertai halaman-halaman yang umumnya diperlukan seperti sampul, lembar pengesahan, kata pengantar, dsb.
- Pembuatan daftar isi, daftar gambar, daftar tabel, dan daftar pustaka secara otomatis.
- Penomoran halaman, gambar, tabel, dan referensi secara otomatis.
- _Input_ gambar dengan format **JPEG**, **PNG**, maupun format lain.
- Pembuatan persamaan, tabel, dan _code snippet_.

## Penjelasan Singkat LaTeX

[**TeX**](https://en.wikipedia.org/wiki/TeX) merupakan salah satu sistem _typesetting_ yang digunakan untuk membuat dokumen secara mudah, dengan format yang konsisten.
**LaTeX** sendiri merupakan salah satu turunan dari **TeX** dengan penambahan lebih banyak fitur dan _package_ yang membantu pembuatan dokumen dengan lebih mudah.
**LaTeX** bersamaan dengan **TeX** sendiri ibaratnya merupakan bahasa pemrograman, agar dapat menghasilkan dokumen yang siap dicetak, diperlukan sebuah _compiler_ yang akan menerjemahkan setiap perintah yang ditulis menggunakan bahasa tersebut.
Untuk saat ini ada beberapa _compiler_ yang bisa digunakan untuk meng-_compile_ **LaTeX**, salah satunya adalah [**TeX Live**](https://www.tug.org/texlive/).
**TeX Live** sendiri dipilih karena alasan _cross-platform_, sehingga bisa digunakan pada sistem operasi yang berbeda, terutama **Windows** dan **Linux**.

## Instalasi TeX Live

Secara umum, cara instalasi dari **TeX Live** bisa dilihat pada halaman utama mereka [disini](https://tug.org/texlive/acquire-netinstall.html).
Namun, karena adanya kebutuhan terhadap _package_ tertentu dari _template_ ini, maka petunjuk ini dibuat sehingga pengguna nantinya cukup menginstall **TeX Live** beserta dengan _package_ tertentu yang dibutuhkan saja.

> Jika anda memilih untuk menggunakan _compiler_ lain seperti [**MikTeX**](https://miktex.org/), [**MacTeX**](https://tug.org/mactex/), dsb. Anda boleh melewati bagian ini.

### Instalasi Menggunakan Installer Untuk Windows

- Unduh _installer_ **TeX Live** untuk **Windows** pada tautan [berikut](http://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe).
- Buka _file_ _installer_ tersebut, kemudian pilih `Install`.
- Jika masih belum muncul bagian instalasi, pilih alternatif _mirror_ `Asia` -> `Singapore`.
- Setelah muncul, pilih bagian `Advanced`.
- Atur `Scheme` menjadi `minimal scheme (plain only)`.
- Klik `Customize`, lalu centang bagian berikut:
  - `Other Languages`.
  - `BibTeX additional styles`.
  - `Essential programs and files`.
  - `LaTeX additional packages`.
  - `LaTeX recommended packages`.
  - `Mathematics, natural sciences, computer science packages`.
  - `Windows-only support programs`.
- Klik `Install` dan tunggu hingga proses instalasi selesai.

### Instalasi Menggunakan APT Linux

- Gunakan perintah berikut untuk melakukan instalasi **TeX Live** pada **Linux**:
  ```bash
  ~$ sudo apt install \
    texlive-latex-extra \
    texlive-lang-other \
    texlive-bibtex-extra \
    texlive-science
  ```
- Tunggu hingga proses instalasi selesai.

## Integrasi LaTeX Dengan Visual Studio Code

> Jika anda memilih untuk menggunakan _text editor_ maupun _IDE_ lain seperti [**Sublime Text**](https://www.sublimetext.com/), [**Texmaker**](https://www.xm1math.net/texmaker/), [**TeXstudio**](https://www.texstudio.org/), dsb. Anda boleh melewati bagian ini.

- Unduh **Visual Studio Code** pada halaman [berikut](https://code.visualstudio.com/download).
- Buka _file_ yang sudah diunduh dan lakukan instalasi **Visual Studio Code**.
- Setelah instalasi, buka _folder_ dari _template_ ini menggunakan **Visual Studio Code**.
- Sebagai tambahan, anda bisa mengunduh beberapa _extension_ berikut yang bisa membantu selama pembuatan buku menggunakan **LaTeX**:
  - [**LaTeX Workshop**](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop), digunakan sebagai _syntax highlighting_ dan _autocomplete_ untuk _file_ berbasis **LaTeX**.
  - [**vscode-pdf**](https://marketplace.visualstudio.com/items?itemName=tomoki1207.pdf), digunakan untuk membuka _file_ `*.pdf` pada **Visual Studio Code**.
  - [**GitLens — Git supercharged**](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens), digunakan untuk _tracking_ perubahan pada _file_ (jika anda menggunakan **Git**).

## Kompilasi Template Menjadi PDF

- Kompilasi dilakukan menggunakan _terminal_ (**Linux**) atau **Command Prompt**/**PowerShell** (**Windows**) pada direktori dari _template_ ini.
  > Jika menggunakan **Visual Studio Code**, anda bisa membuka _terminal_ langsung pada _menu_ `View` -> `Terminal`.
- Gunakan perintah `pdflatex main.tex` untuk melakukan kompilasi template menjadi **PDF**.
  Terkadang perintah perlu dilakukan beberapa kali (biasanya dua kali) agar semua konten muncul pada **PDF** yang dihasilkan.
- Gunakan perintah `bibtex main.aux` kemudian `pdflatex main.tex` beberapa kali (biasanya dua kali) untuk memunculkan hal yang berhubungan dengan pustaka pada **PDF** yang dihasilkan.

## Cara Menggunakan Template

Bagian utama dokumen terletak pada _file_ `main.tex` yang digunakan untuk mengatur _package_ apa saja yang digunakan serta _file_ lain yang akan di-_inputkan_.
Setelah dilakukan kompilasi, hasilnya akan ada banyak _file_ `main` dengan format yang berbeda.
Yang terpenting adalah _file_ `main.pdf` yang merupakan hasil akhir dari kompilasi dokumen tersebut.

Selain itu ada beberapa bagian lain dari _template_ ini selain `main.tex` yang bisa diubah, seperti:
- **_Folder_ `bab`**, berisi _file_ `*.tex` dari bab yang akan dimasukkan pada buku laporan kerja praktik.
- **_Folder_ `pengesahan`**, berisi _file_ `*.tex` dari lembar pengesahan untuk buku laporan kerja praktik.
- **_Folder_ `sampul`**, berisi _file_ `*.tex` dari sampul luar dan dalam untuk buku laporan kerja praktik.
- **_Folder_ `lainnya`**, berisi _file_ `*.tex` dari halaman lain yang akan dimasukkan pada buku laporan kerja praktik.
- **_Folder_ `gambar`**, berisi _file_ `*.jpg`, `*.png`, maupun format gambar lain yang akan dimasukkan pada dokumen.
- **_Folder_ `tabel`**, berisi _file_ `*.text` dari tabel yang akan dimasukkan pada dokumen.
- **_Folder_ `program`**, berisi _file_ kode program yang akan dimasukkan pada dokumen.
- **_File_ `pustaka/pustaka.bib`**, berisi daftar referensi yang akan dimasukkan pada dokumen.

> Penjelasan lebih lanjut mengenai modifikasi pada template akan dijelaskan dengan _comment_ yang bisa dilihat langsung pada masing masing _file_ yang tersedia.

## Kontribusi

Karena keterbatasan pengetahuan mengenai aturan yang berlaku di setiap departemen di **ITS** serta agar _template_ yang dibuat ini bisa berkembang dengan fitur yang lebih banyak, diharapkan adanya kontribusi dari pihak lain yang bersedia untuk membantu.
Untuk melakukan kontribusi, siapapun bisa memulai dengan melakukan _fork_ pada repositori utama _template_ ini yang ada di [**b201lab/template-buku-kp-its**](https://github.com/b201lab/template-buku-kp-its), kemudian membuat perubahan dan melakukan _pull request_.
Jika terdapat masalah dari _template_ ini maupun hal yang berkaitan dengan _template_ ini, jangan ragu untuk membuat _issue_ baru pada halaman _issues_ yang bisa diakses [disini](https://github.com/b201lab/template-buku-kp-its/issues).