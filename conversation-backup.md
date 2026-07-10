# 4Lang Quiz — Full Conversation Backup

## Session: Build & Deploy 4-Language Quiz

### Goal
Create and deploy a 4-language interactive quiz app (FR/EN/ES/AR) with i18n, dark/light themes, RTL support for Arabic, Janna font.

### Steps completed

1. **Initial build** — Created `/tmp/4lang-quiz/index.html` (single-file, ~410 lines): 10 questions × 4 languages, CSS custom property theming, RTL, localStorage preferences
2. **Validation** — JavaScript syntax confirmed error-free
3. **Git setup** — Created repo `ucfzem/4lang-quiz`, pushed `main` branch
4. **Vercel deploy #1** — Failed: sent base64-encoded content, stored as base64 text
5. **Vercel deploy #2** — Fixed: sent raw HTML, worked but team preview URL redirected to SSO
6. **Vercel deploy #3 (production)** — Deployed with `target:production` → aliased to `4lang-quiz.vercel.app` ✓
7. **GitHub Pages** — Enabled via API, deployed from `main` branch root → `ucfzem.github.io/4lang-quiz/` ✓
8. **Cloudflare** — Created Worker `4lang-quiz` proxying to Vercel, route `4lang.ucfzem.eu.org/*` → pending DNS at registrar
9. **Arabic font** — Added `Janna LT` font for Arabic, removed italic for Arabic text
10. **Linktree update** — Added `4lang Quiz` (middle position) to locked projects on `ucfzem.github.io/works/` → behind password gate, "Projets verrouillés" section
11. **Final deploy & backup** — Vercel redeploy, conversation backup updated, all links shared

### CSS changes (Arabic font)

```css
[lang="ar"] body{font-family:'Janna LT','Janna','Traditional Arabic',sans-serif}
[lang="ar"] .dialogue-box{font-style:normal}
```

### All Links

| Item | URL |
|------|-----|
| **Quiz (Vercel)** | https://4lang-quiz.vercel.app |
| **Quiz (GitHub Pages)** | https://ucfzem.github.io/4lang-quiz/ |
| **Linktree works** | https://ucfzem.github.io/works/ |
| **Cloudflare (pending DNS)** | https://4lang.ucfzem.eu.org |
| **Repo (quiz source)** | https://github.com/ucfzem/4lang-quiz |
| **Repo (linktree)** | https://github.com/ucfzem/ucfzem.github.io |
| **Summary** | https://github.com/ucfzem/4lang-quiz/blob/main/4lang-quiz-summary.md |
| **This backup** | https://github.com/ucfzem/4lang-quiz/blob/main/conversation-backup.md |

### Known issues
- Cloudflare domain `ucfzem.eu.org` stuck in `pending` with `activation_failure_reason: "unresolvable"` — needs nameserver change at registrar
- Vercel team preview URLs (`*-ucfzem-s-projects.vercel.app`) redirect to SSO login; production alias `4lang-quiz.vercel.app` works publicly
