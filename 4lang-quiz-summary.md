# 4Lang Quiz — Project Summary

## What was built
A 4-language interactive quiz app (French, English, Spanish, Arabic) featuring:
- i18n translations for all UI and question content
- Dark/light theme toggle (dark default: brown/gold/yellow/white; light: beige/brown/gold)
- RTL layout for Arabic
- Janna font for Arabic text (no italic for Arabic)
- 10 real-life situation questions per language (café, station, hotel, restaurant, pharmacy, taxi, museum, phone, luggage, bakery)
- Progress dots, score tracking, feedback on each answer
- Single-file HTML (no build step needed)

## Deployments
| Platform | URL |
|----------|-----|
| **GitHub Pages** | https://ucfzem.github.io/4lang-quiz/ |
| **Vercel** | https://4lang-quiz.vercel.app |
| **Cloudflare** | https://4lang.ucfzem.eu.org (pending DNS — user must set nameservers at registrar) |

## Technical details
- **File:** `/tmp/4lang-quiz/index.html` — single self-contained HTML (CSS + JS inline)
- **Stack:** Vanilla HTML/CSS/JS, no framework
- **Repo:** https://github.com/ucfzem/4lang-quiz
- **Vercel project:** `4lang-quiz` under team `ucfzem-s-projects`
- **Cloudflare:** Worker `4lang-quiz` routes through `4lang.ucfzem.eu.org`

## How to update
1. Edit `/tmp/4lang-quiz/index.html`
2. Commit & push to GitHub → auto-deploys to GitHub Pages
3. Run Vercel deployment script with raw HTML content (see agent conversation)

## Key files
- `index.html` — the full quiz application
- `4lang-quiz-summary.md` — this file
