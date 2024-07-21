# Landing Page Boilerplate

Projek ini adalah boilerplate untuk membangunkan laman web landing page menggunakan Bootstrap versi 5.3.3, Sass, dan JavaScript. Projek ini disusun dengan struktur folder yang jelas dan kemas untuk memudahkan pembangunan dan penyelenggaraan.

## Struktur Folder

```plaintext
landingpage-boilerplate/
├── css/                    # Folder untuk fail CSS yang dihasilkan
│   └── app.css             # Fail CSS utama yang dihasilkan oleh Sass
├── js/                     # Folder untuk fail JavaScript
│   └── app.js              # Fail JavaScript utama
├── sass/                   # Folder untuk fail Sass
│   ├── abstracts/          # Folder untuk abstracts (functions, mixins, placeholders, variables)
│   │   ├── _abstracts.scss
│   │   ├── _functions.scss
│   │   ├── _mixins.scss
│   │   ├── _placeholders.scss
│   │   └── _variables.scss
│   ├── base/               # Folder untuk styles asas (animations, reset, typography)
│   │   ├── _base.scss
│   │   ├── _animations.scss
│   │   ├── _reset.scss
│   │   └── _typography.scss
│   ├── components/         # Folder untuk components (buttons, etc.)
│   │   ├── _components.scss
│   │   └── _buttons.scss
│   ├── layout/             # Folder untuk layout styles (footer, forms, grid, navbar, sidebar)
│   │   ├── _layout.scss
│   │   ├── _footer.scss
│   │   ├── _forms.scss
│   │   ├── _grid.scss
│   │   ├── _navbar.scss
│   │   └── _sidebar.scss
│   ├── pages/              # Folder untuk styles khusus halaman (home, etc.)
│   │   ├── _pages.scss
│   │   └── _home.scss
│   ├── themes/             # Folder untuk theme styles
│   │   ├── _default.scss
│   │   └── _themes.scss
│   ├── vendors/            # Folder untuk vendor styles
│   │   └── _vendors.scss
│   ├── _settings.scss      # Fail untuk settings Sass
│   └── app.scss            # Fail Sass utama
├── index.html              # Fail HTML utama
├── package.json            # Fail konfigurasi npm
└── README.md               # Panduan projek ini

```

## Cara Menggunakan

1. Muat Turun Projek

Clone atau muat turun projek ini:

```sh
git clone https://github.com/yourusername/landingpage-boilerplate.git
cd landingpage-boilerplate
```

2. Pasang Dependencies

   Pastikan anda telah memasang Node.js. Kemudian, pasang dependencies:

   npm install

3. Struktur Sass

   Fail sass/app.scss adalah fail Sass utama yang mengimport semua sub-fail yang lain:

   @import "settings";
   @import "abstracts/abstracts";
   @import "base/base";
   @import "components/components";
   @import "layout/layout";
   @import "pages/pages";
   @import "themes/themes";
   @import "vendors/vendors";

   @import "../node_modules/bootstrap/scss/bootstrap";

4. Menjalankan Pengawasan Sass
   npm run dev
