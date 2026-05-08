# 👁️ Prompt: POV Knight Battle (15-second First-Person)

[← Back to drama prompts](README.md)

> Format viral Q2/2026 — first-person POV continuous shot, camera = nhân vật's eyes. Single shot không cuts.

---

## 📋 Spec

| Property | Value |
|----------|-------|
| Format | POV / Orb |
| Aspect | 9:16 (TikTok) hoặc 16:9 (YouTube) |
| Duration | 15s |
| Difficulty | Intermediate |
| Cost estimate | ~$3-4 |
| Platform | 0ai.vn hoặc Jimeng |

---

## 🎯 Concept

Camera = mắt của một knight chuẩn bị vào trận chiến. Người xem trải nghiệm POV first-person liên tục: nhìn xuống tay cầm kiếm, nhìn ra trận địa, đối mặt enemy, raise sword, attack. Single continuous shot 15 giây không cuts.

---

## 🎨 Reference Image (Optional)

Nếu dùng reference image, generate 1 ảnh:
- POV view down at gauntlet hand holding sword
- Foreground: armored hand, blade visible
- Background: misty battlefield
- First-person perspective

Use FLUX 1.1 Pro for armor/blade material detail.

---

## 🎬 Motion Prompt (3-Layer)

```
STYLE & MOOD:
First-person POV battle scene. Medieval knight on misty battlefield. 
15-second continuous unbroken shot. Cinematic, "1917" aesthetic meets "Mount and Blade" 
gameplay realism. 9:16 vertical for TikTok (or 16:9 for YouTube — generate both).
24fps. Color: muted earth tones with cold mist + warm sun pierce.

DYNAMIC DESCRIPTION:
SINGLE CONTINUOUS POV SHOT. Camera is the knight's eyes — viewer experiences 
everything first-person. No cuts. No camera switches. Pure first-person continuous.

0-3s: Looking down at hands. Right hand grips medieval longsword (steel blade, 
leather-wrapped grip, basket hilt). Left hand on horse reins. Steel gauntlets visible. 
Subtle breath rise/fall implies POV character breathing.

3-6s: Camera tilts up slowly. Mist parts. Battlefield reveals — 
field with banners, dim shapes of enemy infantry 50m away. 
Distant war drums.

6-9s: Camera scans left-right slowly, surveying scene. 
Enemy commander visible in distance. Ally to right also on horseback.

9-11s: Camera focus shifts to lead enemy charging toward POV. 
Sword raises into frame, vertical, ready position.

11-13s: Enemy reaches striking distance. Sword swings forward 
in defensive arc. Clash of steel sound. Sparks visible.

13-15s: Enemy falls or recoils. Camera scans for next threat. 
Final beat: looking forward at battlefield, more enemies coming.

STATIC DESCRIPTION:
POV consistency LOCKED throughout — same hands, same sword, same gauntlets visible 
in every frame they appear. NO camera identity break. NO third-person cuts.

Setting: misty medieval battlefield, consistent geography. 
Lighting: overcast with periodic sun pierce, cool gray-blue base + warm gold accent.

HARD CONSTRAINTS:
- Single continuous shot — NO cuts allowed
- POV camera identity strict — never switches to third-person
- Hands/sword physical accuracy in close foreground
- Sword must respect physics during swing (no clipping, no morphing)
- Background battlefield maintains spatial logic (banners stay positioned)
- Mist physics realistic (doesn't disappear/teleport)

AUDIO:
- Heavy breathing of POV character (audible)
- Ambient: distant war drums, muffled enemy yells
- Foley: leather creak from gauntlets, sword cutting air, hoof beats
- Climactic: steel-on-steel clash at 11-13s
```

---

## 🎯 Variations

### Variation A: Vietnamese cổ trang version
Replace "medieval knight" with "Vietnamese soldier Trần dynasty defending against Mongols". 
Wardrobe: giáp lá tre (bamboo armor), kiếm Đông A. Setting: Bạch Đằng riverbank.

### Variation B: Sci-fi
Replace medieval with cyberpunk samurai. HUD overlay visible at edges of POV.

### Variation C: Modern
First-person POV of skateboarder navigating Saigon traffic. Same continuous-shot principle.

---

## 🚨 Common Issues

### Issue 1: Camera breaks POV mid-video
**Cause:** Seedance defaults to third-person at climax.
**Fix:** Strengthen prompt — "STRICTLY first-person POV from start to end. NO third-person reveals. NO cuts to outside view."

### Issue 2: Sword glitches during swing
**Cause:** Fast motion causes physics issues.
**Fix:** Add "Sword movement smooth, controlled, no clipping or morphing artifacts during action peak."

### Issue 3: Hands look fake
**Cause:** Hands are hardest part for AI.
**Fix:** Reference image with FLUX 1.1 Pro hand detail. Or: "Hands clearly show 5 fingers, gauntlets articulated correctly at joints."

---

## 🔗 Related

- [Scene Archetype Router](../../resources/05-archetype-router.md) — ACTION archetype
- [Henshin Prompt](21-henshin-samurai.md) — similar transformation feel
- [16-Panel Short Film Master](../../workflows/02-grid-16-panel/04-short-film.md)

---

[← Drama Prompts](README.md) · [Main README](../../README.md)
