# 4Lang Quiz — Full Conversation Backup

## Session: Build & Deploy 4-Language Quiz

### Goal
Create and deploy a 4-language interactive quiz app (FR/EN/ES/AR) with i18n, dark/light themes, RTL support for Arabic, Janna font.

### Steps completed

1. **Initial build** — Created `/tmp/4lang-quiz/index.html` (single-file, 408 lines): 10 questions × 4 languages, CSS custom property theming, RTL, localStorage preferences
2. **Validation** — JavaScript syntax confirmed error-free
3. **Git setup** — Created repo `ucfzem/4lang-quiz`, pushed `main` branch
4. **Vercel deploy #1** — Failed: sent base64-encoded content, stored as base64 text
5. **Vercel deploy #2** — Fixed: sent raw HTML, worked but team preview URL redirected to SSO
6. **Vercel deploy #3 (production)** — Deployed with `target:production` → aliased to `4lang-quiz.vercel.app` ✓
7. **GitHub Pages** — Enabled via API, deployed from `main` branch root → `ucfzem.github.io/4lang-quiz/` ✓
8. **Cloudflare** — Created Worker `4lang-quiz` proxying to Vercel, route `4lang.ucfzem.eu.org/*` → pending DNS at registrar
9. **Arabic font** — Added `Janna LT` font for Arabic, removed italic for Arabic text

### CSS changes (Arabic font)

```css
[lang="ar"] body{font-family:'Janna LT','Janna','Traditional Arabic',sans-serif}
[lang="ar"] .dialogue-box{font-style:normal}
```

### Deployed URLs
| Platform | URL | Status |
|----------|-----|--------|
| GitHub Pages | https://ucfzem.github.io/4lang-quiz/ | ✅ Live |
| Vercel | https://4lang-quiz.vercel.app | ✅ Live |
| Cloudflare | https://4lang.ucfzem.eu.org | ⏳ Pending DNS (set nameservers: `colette.ns.cloudflare.com` / `lennon.ns.cloudflare.com`) |

### Repo
https://github.com/ucfzem/4lang-quiz
(main branch, single-file, no build step)

### Known issues
- Cloudflare domain `ucfzem.eu.org` stuck in `pending` with `activation_failure_reason: "unresolvable"` — needs nameserver change at registrar
- Vercel team preview URLs (`*-ucfzem-s-projects.vercel.app`) redirect to SSO login; production alias `4lang-quiz.vercel.app` works publicly
- GitHub Pages uses the `ucfzem.github.io/4lang-quiz/` project site URL
