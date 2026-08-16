# MAIN "Asli atau AI?" : Deploy Guide

One file, zero build step, zero backend. Everything below takes ~20 minutes total.

## 1. Add the photo rounds (10 min)
The game is playable immediately with 12 text items. Photo rounds unlock when these 4 files exist next to index.html:

```
assets/ai-01.jpg     <- AI-generated (use Aldo's Stable Diffusion pipeline)
assets/ai-02.jpg     <- AI-generated
assets/real-01.jpg   <- real photo you own or have permission to use
assets/real-02.jpg   <- real photo
```

Tips: JPG, roughly 800x600, under 300KB each. Good AI subjects: a person at a market, food, a landscape. Make them believable, not obviously fake; the game is supposed to be hard. Do NOT use real people's faces without consent, and do not depict real public figures.

## 2. Test locally (1 min)
Just open index.html in a browser. If images do not load via file://, run:
```
python -m http.server 8000
```
and open http://localhost:8000

## 3. Deploy (pick one, ~5 min)

**GitHub Pages**
1. Create a public repo (e.g. main-game)
2. Upload index.html + the assets folder
3. Settings > Pages > Source: main branch, root
4. URL: https://USERNAME.github.io/main-game/

**Hugging Face Spaces**
1. New Space > SDK: Static
2. Upload index.html + assets folder
3. URL: https://huggingface.co/spaces/USERNAME/main-game

## 4. Finish the proposal (5 min)
- Paste the live URL into the cover table and section 5.8
- Take 3 screenshots and insert them in section 5.8:
  1. Start screen
  2. A chat card mid-swipe (ghost stamp visible)
  3. The Teachable Moment sheet after an answer
- Fill remaining yellow placeholders (ages, roles, gender balance sentence, verify Ari's spelling)
- File > Export as PDF, confirm under 10MB

## 5. Record the video
Follow MAIN_Pitch_Video_Script.md. The demo scene is a screen recording of this game on a phone.

## 6. Submit
https://tally.so/r/MePkYk before 23:59 Paris time (04:59 WIB / 05:59 WITA). Aim for 2 hours early. Screenshot the confirmation.
