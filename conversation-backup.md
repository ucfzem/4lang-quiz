# Session — Currency DH + درهم smaller

## What was done
- Changed all prices from EUR to DH/MAD
  - 19,99€ → 200 DH / 200 درهم
  - 29,99€ → 300 DH / 300 درهم
  - 49,99€ → 500 DH / 500 درهم
- Split price into `num` + `cur` keys for separate styling
- Added `.price-cur { font-size: .6em }` so "درهم" and "DH" render smaller than the number
- Added `/mes` for Spanish and `/شهر` for Arabic month labels
- All 4 languages (FR/EN/ES/AR) updated

## Files changed
- `/tmp/gh-pages/sport/index.html`: price HTML + i18n keys + CSS

## Links
- **Vercel**: https://ucfzem-works.vercel.app/sport/
- **GitHub Pages**: https://ucfzem.github.io/sport/
- **Works link tree**: https://ucfzem-works.vercel.app/works/
- **GitHub repo**: https://github.com/ucfzem/ucfzem.github.io
