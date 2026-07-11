# Session Backup — 11 July 2026

## Summary
- **VoiceForge**: Refactored v4 with `committedSegments` dedup, `setRecordingUI`, `createRecognitionInstance`, `normalizeForCompare`. Fixed Android stop button (Lucide SVG DOM), restart creates fresh `SpeechRecognition` instance on `onend`, restart delay 300ms→50ms, removed "Reconnecting..." message.
- **Liens 404**: Built an interactive click-miss button — sits calmly, teleports on mousedown, taunts in French, requires 6 catches before surrendering with a working link to /works/.
- **Works page**: Bumped locked projects opacity 0.3→0.5, text 0.15→0.4, grayscale 100%→60% for better readability while still clearly locked.
- **4lang-quiz v2 fixes**: Removed `.container { overflow: hidden }`, fixed `applyUI` Arabic title, restart via `addEventListener`, removed double `showQ()`, added `touch-action: manipulation`, `window.scrollTo` in showQ/nextQ.

## Repos & Links
| Project | Vercel | GitHub Pages | Repo |
|---|---|---|---|
| VoiceForge | https://voiceforge-delta.vercel.app | - | https://github.com/ucfzem/VoiceForge |
| Works | https://ucfzem-works.vercel.app | https://ucfzem.github.io/works/ | https://github.com/ucfzem/ucfzem.github.io |
| 4lang Quiz | https://4lang-quiz.vercel.app | https://ucfzem.github.io/4lang-quiz/ | https://github.com/ucfzem/4lang-quiz |
| Liens 404 | - | https://ucfzem.github.io/liens/ | https://github.com/ucfzem/liens |

## Commits Today
- liens: `28d0871` — Simple click-miss button
- liens: `59cbe98` — Fix navigation when done
- liens: `e780737` → `c4d8a48` → `28d0871` → `59cbe98` (iterations on 404)
- works: `d2819fc` — Locked projects opacity adjustment
- 4lang-quiz: `06f973e` — Backup update
- voiceforge: `9409541`, `c718ffb` — v4 refactor + deploy

## Credentials
- Vercel token: ✓ (set in env)
- GitHub token: ✓ (set in env)
- Cloudflare password: ✓ (stored securely)
