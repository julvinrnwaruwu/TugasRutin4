# Tugas Rutin 4 — Konversi CSS ke SCSS

Project ini mengonversi CSS portofolio dari Tugas Pertemuan 2 ke SCSS modular menggunakan pola 7-1.

## Struktur

```text
scss/
├── abstracts/
├── base/
├── components/
├── layout/
├── pages/
├── themes/
└── vendors/
```

## Requirement yang dipenuhi

1. CSS existing dikonversi ke SCSS.
2. Variables digunakan untuk warna, spacing, radius, dan ukuran layout.
3. Nesting diterapkan dengan kedalaman maksimal 3 level.
4. Ada minimal 3 mixin reusable:
   - `card`
   - `respond`
   - `form-control`
5. Struktur 7-1 pattern digunakan.
6. Semua modularisasi memakai `@use`, bukan `@import`.
7. Perulangan `@each` digunakan pada `pages/_sections.scss`.
8. Project dapat di-compile menggunakan Dart Sass atau dijalankan dengan Vite.

## Compile dengan Dart Sass

Pastikan Node.js dan npm sudah terpasang.

```bash
npm install
npm run sass
```

Hasil compile berada di:

```text
css/main.css
```

Untuk mode otomatis:

```bash
npm run sass:watch
```

## Jalankan dengan Vite

```bash
npm install
npm run dev
```

Untuk build production:

```bash
npm run build
```

## Catatan

`index.html` sudah diarahkan ke `css/main.css`, sehingga hasil compile Dart Sass dapat langsung digunakan.
