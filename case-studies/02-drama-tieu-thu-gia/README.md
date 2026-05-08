# Case Study 02: Drama "Tiểu Thư Giả" (12-Panel Grid)

[← Back to case studies](../README.md)

> Vertical drama short cho TikTok webnovel adaptation. 12-panel custom (not 9 hoặc 16) for narrative pacing.

---

## 📝 Brief (Anonymized)

```
Client: Indie webnovel publisher VN, adapting popular novel
Brief tiếng Việt:
"Cần video 12 giây promote drama 'Tiểu thư giả' — câu chuyện về 
cô gái nghèo giả tiểu thư để trả nợ. Cảnh: cô đến biệt thự nhà giàu, 
bị soi mói, lộ chân tướng. Cuối cùng đứng vững. 
Format dọc 9:16. Ngân sách: 8 triệu."

Deliverable: 12-second vertical drama promo, 1080p, with subtitles option
```

---

## 🎯 Approach

- **Archetype:** PORTRAIT + ACTION hybrid
- **Workflow:** Custom **12-panel grid** (4 rows × 3 cols) — middle ground between 9 and 16
- **Why 12 not 9 or 16?** 12 seconds video needs ~12 beats. 9 too compressed, 16 too stretched.
- **Models:** GPT Image 2 (layout) + Nano Banana 2 (face fidelity Asian)
- **Total time:** 2 hours
- **Production cost:** ~$8

---

## 🎨 Custom 12-Panel Beat Structure

| Block | Panels | Function |
|-------|:------:|----------|
| Setup (1-3) | Cô đến biệt thự, được đón bằng nghi thức | Establish stakes |
| Inspection (4-6) | Bị các "thật tiểu thư" soi từng chi tiết | Tension builds |
| Reveal (7-9) | Một chi tiết lộ — vết chai tay, đôi giày sờn | Crisis |
| Resolution (10-12) | Cô không gục — đứng thẳng, nói lời sắc bén | Empowerment |

---

## 🎨 Grid Storyboard Prompt

```
A 4×3 grid storyboard (1:1 aspect, 12 cinematic panels with bold black 4px borders 
and 8px white gutters). Vietnamese vertical drama short, webnovel adaptation.

ULTRA-CONSISTENT CHARACTER A (@subject1): A 23-year-old Vietnamese woman, 
163cm slim, Northern accent feel.
Hair: dark brown long wavy, pulled half-up with simple gold pin, 
slight imperfection (one strand falling on cheek).
Face: heart-shaped, large doe eyes, fair-pale skin slightly sun-touched, 
defined cupid's bow lips natural rose color, single small mole near left lip.
Wardrobe: borrowed-looking but expensive — pale pink silk áo dài modern cut, 
slight wrinkle at hem (sign of borrowing). Pearl earrings small. 
Watch hidden under sleeve. Hands show subtle calluses (lying about being rich).

ULTRA-CONSISTENT CHARACTER B (@subject2): "Real" tiểu thư, 25 tuổi.
Hair: glossy black sleek bob to chin, perfect.
Face: angular, intimidating, immaculate makeup, condescending micro-smile.
Wardrobe: red silk áo dài haute couture, ruby earrings, designer watch visible.

Setting: Modern Vietnamese luxury villa interior. Marble floors, 
crystal chandelier, family altar with golden Buddha, traditional artwork on walls.
Late afternoon light through tall windows.

Read panels left-to-right, top-to-bottom (4 rows × 3 cols):

ROW 1 (Setup):
Panel 1: WIDE. Character A enters villa entrance, intimidated but composed. 
Servants bow. She tries not to look impressed.

Panel 2: MEDIUM. Character B descends marble staircase, condescending smile. 
Other 2 women behind her, judging.

Panel 3: ECU. Character A's hand discreetly smoothing her áo dài. 
Subtle calluses visible (the tell).

ROW 2 (Inspection):
Panel 4: MEDIUM 2-shot. Character B circles Character A, examining outfit.

Panel 5: CLOSE-UP on Character B's eyes — narrowed, predatory.

Panel 6: ECU. Character B's eyes glance down at Character A's shoes — 
worn at heel, poor quality leather. Tell #2.

ROW 3 (Reveal):
Panel 7: MEDIUM. Character B's mouth opens to speak, finger pointing at shoes.

Panel 8: WIDE 2-shot. Other women now staring, smirks growing.

Panel 9: CLOSE-UP on Character A's face. Realization. Vulnerability for one second.

ROW 4 (Resolution):
Panel 10: CLOSE-UP. Character A's expression hardens. Resolve.

Panel 11: MEDIUM. She straightens her back. Looks Character B directly in the eye.

Panel 12: WIDE. Character A stands tall, head slightly lifted. 
Character B's smile falters. The other women shift uncomfortably.

STYLE REQUIREMENTS:
- Modern Vietnamese drama, vertical TikTok webnovel adaptation aesthetic
- Reference: "Phượng Khấu" period drama meets contemporary K-drama
- Color script: warm gold establish, cool blue tension, warm ember resolution
- Vertical-friendly composition (subject centered)
- AVOID: cheap soap opera lighting, over-saturation, generic "Asian drama"

CHARACTER FIDELITY ABSOLUTE — both characters' faces identical across all panels.
```

---

## 🎬 Motion Prompt (Seedance)

[Available trong full case study walkthrough — request in [Zalo community](https://zalo.me/g/caqqva644)]

---

## 📊 Result

- Duration: 12.0s
- Resolution: 1080×1920 (TikTok native vertical)
- Audio: Vietnamese voiceover narration + dramatic underscore
- Posted by client: 380K views first 24h, 2.1M views first week

---

## 💰 ROI Breakdown

| Item | Cost |
|------|:----:|
| GPT Image 2 grid (3 iterations) | $1.20 |
| Nano Banana 2 face fidelity (5 cells) | $0.80 |
| Seedance 480p tests (4 versions) | $2.00 |
| Seedance 1080p final (2 versions) | $5.00 |
| Audio + voiceover | $1.50 |
| Editing time CapCut Pro | (your time, ~45 min) |
| **Total cost** | **~$10.50** |
| **Client paid** | **8,000,000 VND (~$320)** |
| **Margin** | **97%** |

**Time invested:** 2 hours
**Effective hourly rate:** ~$155/hr

---

## 📝 Lessons Learned

### What worked
✅ **12-panel custom grid** — perfect for 12s drama, neither 9 nor 16 was right
✅ **Subtle "tells" in Character A** (calluses, worn shoes, hidden watch) — visual storytelling
✅ **Color script evolution** — viewer feels emotion shift even without dialog

### What didn't work first try
❌ **Character B initially looked too similar to A** — increased contrast (red vs pink, sleek vs wavy)
❌ **First grid had Character A looking too impoverished** — softened with "expensive borrowed" not "poor"
❌ **Initial 1080p had aspect issues** — had to regenerate with explicit 1:1 grid spec

### Key insight
Vertical drama works because of **face-forward composition + emotional close-ups**. Drop wide establishing shots from the middle, keep them only at edges (panel 1, 12).

---

## 🔗 Related

- [9-Panel Workflow](../../workflows/01-grid-9-panel.md) — Default version
- [Character Bible System](../../workflows/03-character-bible.md) — Multi-character setup

---

[← Case Studies](../README.md) · [Main README](../../README.md)
