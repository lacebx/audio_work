# audio_work — AI Voice & Audio Experiments

Before I knew what "AI engineering" even was as a career path, I was already experimenting with it. `audio_work` is a collection of audio files from a 2023 session where I was exploring AI voice synthesis, stem separation, and audio enhancement tools.

The workflow was simple but genuinely fascinating: take a song, strip it into its component parts (music + vocals), enhance the vocal track, then layer in AI-generated voice using ElevenLabs with a custom voice profile I named **Arsene**.

> *Birarenze* — when curiosity about AI meets a love of music, this is what happens.

---

## The Workflow

```
Original Track
    ↓
[Vocali.se] — AI-powered stem separation
    ├── [music].mp3    (instrumental track)
    └── [vocals].mp3   (isolated vocals)
         ↓
    [enhanced]     (vocal cleanup/enhancement)
         ↓
[ElevenLabs] — AI voice generation (Arsene profile)
    └── ElevenLabs_..._Arsene_ivc_*.mp3
```

---

## Files Breakdown

| File | Description |
|------|-------------|
| `spotifydown.com - Chicago Freestyle (feat. Giveon).*` | Original source track split into music/vocals |
| `spotifydown.com - Moment Of Truth.mp3` | Full source track |
| `audio [music].mp3` | Separated instrumental |
| `audio [vocals] (enhanced).mp3` | Isolated + enhanced vocal track |
| `filtered-*.mp3` | Filtered versions of separated stems |
| `ElevenLabs_2023-09-22T*_Arsene_ivc_*.mp3` | AI-generated voice outputs (Arsene voice clone) |
| `Vocali.se_2204.zip` | Vocali.se stem separation tool |

---

## Tools Used

- **[Vocali.se](https://vocali.se)** — AI audio stem separator (vocals/music isolation)
- **[ElevenLabs](https://elevenlabs.io)** — AI voice synthesis (voice cloning, IVC)
- **Custom voice profile:** Arsene (trained/configured personally)

---

## Why This Exists

I was curious whether I could build a full audio pipeline using AI tools — take a song I liked, deconstruct it, and rebuild parts of it with my own voice or an AI voice. The ElevenLabs files here are generated with specific parameters (`s20/s28`, `sb100`, `se20/se33`) that control stability and similarity to the source voice. It was hands-on learning at its best.
