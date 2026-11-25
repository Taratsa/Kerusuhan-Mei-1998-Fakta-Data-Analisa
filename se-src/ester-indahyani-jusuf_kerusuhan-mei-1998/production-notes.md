# Catatan produksi

- Sumber dan keterangan edisi: lihat `se-imprint.md` dan `se-colophon.md` (dapat disunting langsung). Teks berasal dari OCR (TurboOCR), bukan dari ketik ulang.
- Naskah dibaca langsung dari `book.md`; edisi ini dibangun ulang dengan `pipeline.py --steps se`.
- Koreksi OCR hanya pada kesalahan yang jelas (pemeriksa ejaan SymSpell, ditinjau manual). Ejaan lama dan tidak baku dari narasumber dipertahankan.
- Kutip lurus dan kutip tunggal diubah menjadi kutip lengkung ganda sesuai manual SE; titik dan koma ditaruh di dalam tanda kutip.
- Singkatan ditulis tanpa titik sesuai kaidah Indonesia dan ditandai z3998:acronym; aturan lint s-023 (kapitalisasi judul gaya Inggris) tidak berlaku untuk bahasa Indonesia.
- Edisi white-label, bukan rilis Standard Ebooks: tanpa logo atau klaim SE. Halaman lisensi menggantikan Uncopyright SE karena teks sumber tidak berada di domain publik.
- Label navigasi (Daftar Isi, Penanda, Halaman Judul) diterjemahkan setelah `se build`; sumber tetap sesuai SE agar `se lint` lolos.
- Teks disalin dari pindaian PDF terbitan SNB dan APHI (2005) dengan OCR; kesalahan OCR diperbaiki seperlunya.
- Tabel dipertahankan sebagai tabel HTML; sebagian sel hasil OCR belum sepenuhnya rapi.
- Catatan kaki tetap berada di akhir halaman aslinya di dalam alur teks, belum disusun sebagai catatan akhir.
