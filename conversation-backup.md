# Session — Solid gold buttons #C5A059 + Arabic coach names + DH currency

## What was done
- Buttons: replaced gradient `var(--gold-grad)` with solid `#C5A059`
  - `.btn-primary`: gold filled (#C5A059 bg, #1A1A1A text, no border)
  - `.btn-outline`: gold outlined (transparent bg, #C5A059 border/text)
  - `.btn-dark`: kept text-based outline
  - Added base `.btn` class with shared properties (padding 15px 30px, border-radius 50px, etc.)
- Arabic coach names: Sarah → سارة, Julien → حسن, Myriam → مريم (with `data-i18n` keys)
- Price split into `num` + `cur` keys, `.price-cur { font-size: .6em }` for smaller درهم/DH
- Currency changed from € to DH (200/300/500)

## Files changed
- `/tmp/gh-pages/sport/index.html`: button CSS, coach HTML, i18n keys, price structure

## Links
- **Vercel Sport**: https://ucfzem-works.vercel.app/sport/
- **GitHub Sport**: https://ucfzem.github.io/sport/
- **Works**: https://ucfzem-works.vercel.app/works/
- **4lang-quiz**: https://4lang-quiz.vercel.app
- **VoiceForge**: https://voiceforge-delta.vercel.app
- **liens**: https://ucfzem.github.io/liens/
- **GitHub repo**: https://github.com/ucfzem/ucfzem.github.io
- **Backup**: https://github.com/ucfzem/4lang-quiz/blob/main/conversation-backup.md
