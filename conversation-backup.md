# Session — Audio fixes + chimes instead of TTS

## What was done
- Drone volume boosted 0.025 → 0.3 (12× louder, clean 220Hz sine)
- Replaced Web Speech TTS with musical chime cues (440Hz شهيق, 220Hz زفير, 660Hz start, 880Hz done)
- Removed duckDrone/unduckDrone (no longer needed without TTS)
- Removed Arabic voice loading code
- Drone fade-in/out with `setValueAtTime` + `linearRampToValueAtTime` (no clicks)
- `playChime()` creates a fresh AudioContext per chime, auto-closes after duration
- Julien → Hassan in all 4 languages

## Files changed
- `/tmp/gh-pages/sport/index.html`

## Links
- **Vercel Sport**: https://ucfzem-works.vercel.app/sport/
- **GitHub Sport**: https://ucfzem.github.io/sport/
- **Works**: https://ucfzem-works.vercel.app/works/
- **4lang-quiz**: https://4lang-quiz.vercel.app
- **VoiceForge**: https://voiceforge-delta.vercel.app
- **liens**: https://ucfzem.github.io/liens/
- **GitHub repo**: https://github.com/ucfzem/ucfzem.github.io
- **Backup**: https://github.com/ucfzem/4lang-quiz/blob/main/conversation-backup.md
