# Session — Audio fixes + drone volume boost

## What was fixed
1. **Julien → Hassan** in ALL 4 languages (FR/EN/ES/AR)
2. **Meditation audio crackle**:
   - 110Hz → 220Hz (cleaner on phone speakers)
   - Volume: 0.025 → 0.08 (louder drone)
   - Duck: 0.008 → 0.025 (still audible under voice)
   - Voice ducking: drone lowers when speech speaks, rises after
   - Arabic voice detection via `onvoiceschanged`
   - Clean fade in/out ramps (no clicks/pops)
   - No double-start AudioContext guard
3. **All modals**: article "5 mistakes", BMR/TDEE calculator, 10min breathing meditation with audio

## Files changed
- `/tmp/gh-pages/sport/index.html`: drone frequencies/gain, ducking, voice loading, coach names

## Links
- **Vercel Sport**: https://ucfzem-works.vercel.app/sport/
- **GitHub Sport**: https://ucfzem.github.io/sport/
- **Works**: https://ucfzem-works.vercel.app/works/
- **4lang-quiz**: https://4lang-quiz.vercel.app
- **VoiceForge**: https://voiceforge-delta.vercel.app
- **liens**: https://ucfzem.github.io/liens/
- **GitHub repo**: https://github.com/ucfzem/ucfzem.github.io
- **Backup**: https://github.com/ucfzem/4lang-quiz/blob/main/conversation-backup.md
