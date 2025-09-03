# 🎨 Via Design Tokens

Repository ini berisi **Design Tokens** untuk sistem desain **Via**, yang digunakan sebagai fondasi visual di berbagai brand whitelabel PT. Trans Berjaya Khatulistiwa (TBK).

Tokens ini mencakup warna, tipografi, spacing, border radius, shadow, dan elemen desain lain yang konsisten di seluruh produk.

---

## 📂 Struktur Token

- **core**  
  Token dasar yang bersifat global (warna, font, spacing, dsb).  
  Digunakan sebagai *single source of truth* untuk semua brand.

- **Brand1** & **Brand2**  
  Contoh implementasi token brand (primary color, font family, dll).  
  Setiap brand dapat melakukan override dari token `core`.

- **Aragon/Light Mode** & **Aragon/Dark Mode**  
  Contoh mode tema (light & dark) untuk variasi tampilan.

---

## ✨ Contoh Token

```json
"core": {
  "color": {
    "base": {
      "black": {
        "value": "#000000",
        "type": "color"
      }
    }
  },
  "fontFamilies": {
    "default": {
      "value": "Plus Jakarta Sans",
      "type": "fontFamilies"
    }
  },
  "spacing": {
    "4": {
      "value": "16px",
      "type": "spacing"
    }
  }
}
```

---

## 🎨 Preview Visual

### Warna Dasar
| Nama | Warna | Hex |
|------|-------|-----|
| Black | ![#000000](https://via.placeholder.com/20/000000/000000.png) | `#000000` |
| White | ![#ffffff](https://via.placeholder.com/20/ffffff/000000.png) | `#ffffff` |
| Neutral 700 | ![#404040](https://via.placeholder.com/20/404040/000000.png) | `#404040` |

### Font Family
| Token | Preview |
|-------|---------|
| Default (`Plus Jakarta Sans`) | <span style="font-family:'Plus Jakarta Sans', sans-serif;">The quick brown fox jumps over the lazy dog</span> |
| Serif (`Georgia`) | <span style="font-family:'Georgia', serif;">The quick brown fox jumps over the lazy dog</span> |
| Mono (`Menlo`) | <span style="font-family:'Menlo', monospace;">The quick brown fox jumps over the lazy dog</span> |

### Spacing Scale
| Token | Value |
|-------|-------|
|   1   |   4px |
|   2   |   8px |
|   4   |  16px |
|   8   |  32px |
|  16   |  64px |

---

## 🚀 Cara Menggunakan

1. **Import file JSON** ke dalam tools seperti:
   - [Tokens Studio for Figma](https://tokens.studio)
   - Build system (misalnya Style Dictionary)
   - Framework frontend (React, Vue, dsb)

2. **Mapping token** sesuai kebutuhan:
   - Gunakan `core` sebagai basis
   - Override dengan token brand (`Brand1`, `Brand2`, dll)
   - Terapkan theme (light/dark) bila diperlukan

---

## 🛠️ Roadmap

- [ ] Penambahan semantic tokens
- [ ] Dokumentasi visual (preview color, font, spacing)
- [ ] Integrasi otomatis dengan design system di Figma
- [ ] Export ke format CSS/SCSS/JS

---

## 📖 Lisensi

© 2025 PT. Trans Berjaya Khatulistiwa.  
Hanya untuk penggunaan internal pengembangan produk whitelabel.

---
