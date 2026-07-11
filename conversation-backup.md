# Session Backup — 11 July 2026

## Summary
- **VoiceForge**: Refactored v4 with `committedSegments` dedup, `setRecordingUI`, `createRecognitionInstance`, `normalizeForCompare`. Fixed Android stop button (Lucide SVG DOM), restart creates fresh `SpeechRecognition` instance on `onend`, restart delay 300ms→50ms, removed "Reconnecting..." message.
- **Liens 404**: Built an interactive click-miss button — sits calmly, teleports on mousedown, taunts in French, requires 6 catches before surrendering with a working link to /works/.
- **Works page**: Bumped locked projects opacity 0.3→0.5, text 0.15→0.4, grayscale 100%→60% for better readability while still clearly locked.
- **4lang-quiz v2 fixes**: Removed `.container { overflow: hidden }`, fixed `applyUI` Arabic title, restart via `addEventListener`, removed double `showQ()`, added `touch-action: manipulation`, `window.scrollTo` in showQ/nextQ.
- **Sport page**: Fitness landing page at ucfzem.github.io/sport/. Full i18n (4 langs FR/EN/ES/AR 🇫🇷🇬🇧🇪🇸🇲🇦), RTL for Arabic, dark/light theme toggle (🌙/☀️), responsive 320px→4K, TV remote keyboard nav. Dark: #0d0d0d/gold/white. Light: beige/brown/gold. No layout jumping on language switch. Removed from public projects, kept only in locked section (💪 between VoiceForge and 4lang Quiz). Images replaced with local JPEGs from user (assets/). Also accessible via Vercel at https://ucfzem-works.vercel.app/sport/.

## Repos & Links
| Project | Vercel | GitHub Pages | Repo |
|---|---|---|---|
| VoiceForge | https://voiceforge-delta.vercel.app | - | https://github.com/ucfzem/VoiceForge |
| Works | https://ucfzem-works.vercel.app | https://ucfzem.github.io/works/ | https://github.com/ucfzem/ucfzem.github.io |
| 4lang Quiz | https://4lang-quiz.vercel.app | https://ucfzem.github.io/4lang-quiz/ | https://github.com/ucfzem/4lang-quiz |
| Liens 404 (→ Vercel Works) | - | https://ucfzem.github.io/liens/ | https://github.com/ucfzem/liens |
| **Sport** | — | **https://ucfzem.github.io/sport/** | https://github.com/ucfzem/ucfzem.github.io |

## Commits Today
- liens: `28d0871` — Simple click-miss button
- liens: `59cbe98` — Fix navigation when done
- liens: `3510bee` — Target changed to ucfzem-works.vercel.app/works/
- liens: `e780737` → `c4d8a48` → `28d0871` → `59cbe98` → `3510bee` (iterations on 404)
- works: `d2819fc` — Locked projects opacity adjustment
- works: `f709e9a` — Added Sport fitness page + linked in works
- works: `8e54f4c` — Added Sport to locked projects (middle, VoiceForge ↔ 4lang Quiz)
- works: `c6ee77c` — Sport full i18n (4 langs, RTL, theme toggle, responsive)
- works: `54f9e33` — Removed Sport from public projects, locked only
- works: `d973a36` — Replaced Unsplash images with local JPEGs from user
- 4lang-quiz: `06f973e` → `e8d41ab` → `ad6574c` → `9b0e808` → ... → `ad6574c` (backup updates)
- voiceforge: `9409541`, `c718ffb` — v4 refactor + deploy

## Credentials
- Vercel token: ✓ (set in env)
- GitHub token: ✓ (set in env)
- Cloudflare password: ✓ (stored securely)
