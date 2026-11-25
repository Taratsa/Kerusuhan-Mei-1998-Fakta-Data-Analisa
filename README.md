# Kerusuhan Mei 1998: Fakta, Data & Analisa — EPUB source

Buku *Kerusuhan Mei 1998: Fakta, Data & Analisa — Mengungkap Kerusuhan Mei 1998 Sebagai Kejahatan Terhadap Kemanusiaan*,
disusun oleh Ester Indahyani Jusuf, Hotma Timbul, Olisias Gultom, dan Sondang Frishka; diterbitkan Solidaritas Nusa Bangsa (SNB)
dan Asosiasi Penasehat Hukum dan Hak Asasi Manusia Indonesia (APHI), cetakan pertama November 2005.

Dibuat dari pindaian PDF 450 halaman (OCR via TurboOCR).

## Status

- `Kerusuhan Mei 1998 - Fakta, Data & Analisa.epub`: normal EPUB3, verify PASS, epubcheck 0 errors/warnings.
- Edisi Standard Ebooks belum dibuat: `--steps se` berhenti pada validasi tabel OCR (baris tabel tidak membentuk grid
  persegi) dan sejumlah tanda kutip hasil OCR. Lihat `se-src/` untuk draf yang belum selesai.

## Build

`book.md` is the hand-edited source (`book.json` `"source": "book.md"`). Edit it directly; it is never regenerated.

    cd /Users/sf/Documents/workspaces/pdf-to-epub-turboocr
    python3 pipeline.py "<path to this folder>" --steps build,verify

Do not run the `ocr` or `images` steps for this book.

## Outputs

- `Kerusuhan Mei 1998 - Fakta, Data & Analisa.epub`: normal EPUB (pandoc build)
- `verify.json`, `review.txt`: build checks

## Hand-editable files

- `book.md`: all text, tables and image references
- `metadata.yaml`, `titlepage.html`, `colophon.html`, `license.html`: normal EPUB metadata and pages (optional)
- `se-imprint.md`, `se-colophon.md`, `se-license.md`: Keterangan Edisi, Kolofon and Lisensi pages of the SE edition

## Lineage OCR -> book.md

`ocr/md/pNN.md` (raw OCR, not tracked) -> `book.ocr-original.md` (frozen baseline) -> `book.md`.
`corrections.json` logs every change from the baseline to `book.md` (SymSpell and manual edits, structural cleanup,
paragraph joins) and is written by `corrections.py` only. `python3 corrections.py check <this folder> --scan` replays it
and must pass (505 edits, 787 kept as printed at the time of writing).

The corrections were not compared against the scan images; they rest on SymSpell suggestions, the dictionaries and
sentence context. Catatan kaki masih berada di akhir halaman aslinya di dalam alur teks, belum disusun sebagai catatan akhir.
Tabel dipertahankan sebagai tabel HTML hasil OCR; sebagian sel belum sepenuhnya rapi.

## Rights

The editorial contributions (OCR, proofreading, typesetting, EPUB structure) are dedicated to the public domain under CC0 1.0.
The underlying text and photographs remain with their rights holders (SNB, APHI and the authors); this edition claims no
rights in them.
