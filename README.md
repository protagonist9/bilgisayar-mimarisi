# Bilgisayar Mimarisi: RISC-V Tabanlı Yaklaşım

**Oğuz Ergin** — University of Sharjah

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

---

## Hakkında

Bu kitap, RISC-V buyruk kümesi mimarisi temelinde yazılmış Türkçe bir bilgisayar mimarisi ders kitabıdır. Lisans düzeyinde bilgisayar mühendisliği ve elektrik-elektronik mühendisliği öğrencilerine yönelik olarak hazırlanmıştır.

**Sürekli güncellenen açık kaynak bir kitaptır.** Hata bildirimleri ve katkılar memnuniyetle karşılanır.

## İçindekiler

| Bölüm | Konu | Durum |
|-------|------|-------|
| 1 | Giriş | ✅ Yayında |
| 2 | Başarım | 🔧 Hazırlanıyor |
| 3 | Buyruk Kümesi Mimarisi | 🔧 Hazırlanıyor |
| 4 | Aritmetik Birimler | 🔧 Hazırlanıyor |
| 5 | İşlemci Tasarımı | 🔧 Hazırlanıyor |
| 6 | Boru Hattı | 🔧 Hazırlanıyor |
| 7 | Bellek Hiyerarşisi | 🔧 Hazırlanıyor |
| 8 | Giriş/Çıkış | 🔧 Hazırlanıyor |
| 9 | Çok Çekirdekli İşlemciler | 🔧 Hazırlanıyor |
| 10 | GPU ve Hızlandırıcılar | 🔧 Hazırlanıyor |
| 11 | Güncel Mimariler | 🔧 Hazırlanıyor |
| Ek A | Sayı Sistemleri | 🔧 Hazırlanıyor |
| Ek B | Sayısal Tasarım | 🔧 Hazırlanıyor |
| Ek C | RISC-V Referans | 🔧 Hazırlanıyor |
| Ek D | Pratik Rehber | 🔧 Hazırlanıyor |

## Derleme

Kitabı derlemek için LuaLaTeX gereklidir:

```bash
# Tüm kitabı derle
lualatex ana-kitap.tex
biber ana-kitap
lualatex ana-kitap.tex
lualatex ana-kitap.tex

# Yalnızca belirli bir bölümü derle
# ana-kitap.tex içinde \includeonly satırını düzenleyin
```

### Gereksinimler

- [TeX Live](https://www.tug.org/texlive/) 2024+ veya [MiKTeX](https://miktex.org/) 24.1+
- LuaLaTeX
- Biber (kaynakça yönetimi)

## Atıf

Bu kitabı akademik çalışmalarınızda kullanıyorsanız lütfen aşağıdaki şekilde atıf yapınız:

```bibtex
@book{ergin2026bilgisayar,
  author    = {Ergin, Oğuz},
  title     = {Bilgisayar Mimarisi: RISC-V Tabanlı Yaklaşım},
  year      = {2026},
  publisher = {Açık Erişim},
  url       = {https://github.com/prof-oguzergin/bilgisayar-mimarisi},
  license   = {CC BY-SA 4.0},
  note      = {Sürekli güncellenen açık kaynak ders kitabı}
}
```

## Lisans

Bu eser [Creative Commons Atıf-AynıLisanslaPaylaş 4.0 Uluslararası](https://creativecommons.org/licenses/by-sa/4.0/) lisansı ile lisanslanmıştır.

Özgürce paylaşabilir, uyarlayabilir ve ticari amaçlarla kullanabilirsiniz — uygun atıf yapmanız ve türetilmiş eserleri aynı lisansla paylaşmanız koşuluyla.
