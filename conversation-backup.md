# Session — Arabic coach names + price num/cur split

## What was done
- Arabized coach names:
  - Sarah → سارة
  - Julien → حسن (Hassan)
  - Myriam → مريم
- Added `data-i18n="coach.c[123].name"` to all coach `<h3>` elements
- Added name keys in all 4 languages (FR/EN/ES keep Latin, AR uses Arabic)
- Price split into `num` + `cur` keys with `.price-cur { font-size: .6em }`

## Files changed
- `/tmp/gh-pages/sport/index.html`: coach HTML + i18n keys

## Links
- **Vercel**: https://ucfzem-works.vercel.app/sport/
- **GitHub Pages**: https://ucfzem.github.io/sport/
- **Works**: https://ucfzem-works.vercel.app/works/
- **4lang-quiz**: https://4lang-quiz.vercel.app
- **VoiceForge**: https://voiceforge-delta.vercel.app
- **liens**: https://ucfzem.github.io/liens/
- **GitHub**: https://github.com/ucfzem/ucfzem.github.io
- **Backup**: https://github.com/ucfzem/4lang-quiz/blob/main/conversation-backup.md
