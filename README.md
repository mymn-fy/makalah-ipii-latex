# Template Makalah LaTeX - Prodi Ilmu Perpustakaan dan Informasi Islam

Repositori ini berisi template penulisan makalah resmi untuk Program Studi Ilmu Perpustakaan dan Informasi Islam (IPII) di UIN Antasari Banjarmasin yang telah dikonversi ke dalam format LaTeX. Template ini bertujuan untuk memudahkan mahasiswa dalam menulis makalah dengan format yang rapi, terstruktur, dan konsisten sesuai dengan standar prodi.

## Struktur Dokumen

Template ini dibagi menjadi beberapa file terpisah untuk memudahkan manajemen dan penulisan:

*   **`main.tex`**: File utama (master). Proses kompilasi (build) dilakukan pada file ini. File ini mengatur *package* yang digunakan dan menggabungkan semua bagian makalah.
*   **`cover.tex`**: Berisi format halaman sampul depan (judul, nama, NIM, dosen pengampu, dll).
*   **`kata-pengantar.tex`**: Berisi halaman Kata Pengantar.
*   **`makalah.tex`**: Berisi batang tubuh makalah utama (BAB I Pendahuluan, BAB II Pembahasan, BAB III Penutup).
*   **`referensi.bib`**: File database daftar pustaka/referensi dalam format BibTeX.
*   **`logo_uin_antasari.png`**: File gambar logo universitas yang digunakan pada halaman *cover*.

## Cara Penggunaan

1.  **Prasyarat**: Pastikan Anda telah menginstal distribusi LaTeX di komputer Anda (seperti [TeX Live](https://tug.org/texlive/), [MiKTeX](https://miktex.org/), atau MacTeX). Sangat disarankan untuk menggunakan editor teks yang memiliki dukungan LaTeX yang baik, seperti **VS Code** (dengan ekstensi LaTeX Workshop) atau **TeXstudio**. Sebagai alternatif yang lebih mudah, Anda juga bisa mengunggah seluruh folder ini ke layanan *cloud* seperti **Overleaf**.
2.  **Kompilasi**: Buka file `main.tex` di editor Anda, lalu lakukan proses *build* atau *compile*. Disarankan menggunakan *compiler* `latexmk` atau menggunakan urutan kompilasi: `pdflatex` $\rightarrow$ `biber` (untuk referensi) $\rightarrow$ `pdflatex` $\rightarrow$ `pdflatex`.
3.  **Pengeditan**:
    *   Buka `cover.tex` dan sesuaikan data diri (Nama, NIM, Judul, dll).
    *   Tulis isi makalah Anda dengan mengedit file `makalah.tex`.
    *   Masukkan sumber referensi jurnal atau buku Anda ke dalam `referensi.bib`.

## Penggunaan Kutipan (Sitasi)

Template ini menggunakan gaya sitasi **Chicago Manual of Style 17th Edition**. Manajemen referensi dilakukan menggunakan standar LaTeX. Untuk mengutip referensi, gunakan perintah `\cite{kunci_referensi}` di dalam teks, di mana `kunci_referensi` adalah ID dari referensi yang ada di dalam file `referensi.bib`.
