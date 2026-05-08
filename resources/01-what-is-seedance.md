# 📘 What is Seedance 2.0?

> **Tổng quan ngắn gọn về Seedance 2.0** — model AI video của ByteDance, hiện là 1 trong 3 model T2V/I2V tốt nhất thế giới (cùng với Veo 3 và Kling 2.5).

[← Back to resources](README.md)

---

## 🇻🇳 TL;DR

Seedance 2.0 là model video generation của ByteDance (cha đẻ TikTok), released cuối 2024 và update lớn vào tháng 4/2026. Đây là model VN creator dùng nhiều nhất vì:
- 🇨🇳 Có sẵn trên Jimeng / Dreamina (tools ByteDance owned)
- 🇻🇳 Có sẵn trên 0ai.vn (không cần VPN)
- ⚡ Fast — 8s video render trong 30-60 giây
- 💰 Cost-effective — $0.30-0.50/video 480p, $1.50-3/video 1080p
- 🎬 Audio generation built-in (v2.1+)

---

## 📊 Capabilities

| Feature | Details |
|---------|---------|
| Resolution | 480p Fast / 720p / 1080p Standard / 4K Pro |
| Duration | 5s, 8s, 10s, 12s, 15s |
| Frame rate | 24fps, 30fps cinematic |
| Aspect ratios | 1:1, 16:9, 9:16, 4:3, 2.39:1 |
| Image-to-Video | ✅ Yes (the killer feature) |
| Text-to-Video | ✅ Yes |
| Audio generation | ✅ Yes (v2.1+) |
| Camera control | ✅ Pan, tilt, zoom, dolly, orbit |
| Character consistency | ✅ With reference image |
| Multi-shot | ⚠️ Limited (use grid storyboard method) |

---

## 🔥 Why Seedance vs Veo 3 vs Kling 2.5

### Seedance 2.0 strengths
- Best **price-performance ratio** ($1.50-3/video 1080p)
- Best **Asian face consistency** (trained heavily on Asian data)
- Best **integration với image-to-video** workflow
- Available ở VN không cần VPN (qua 0ai.vn)

### Veo 3 strengths
- Better English text rendering (signs, captions)
- More photorealistic in some Western contexts
- Higher max resolution potential
- BUT: more expensive ($5-15/video), Google ecosystem only

### Kling 2.5 strengths
- Best slow-motion physics
- Best fluid simulation (water, smoke)
- BUT: cũng cần VPN cho VN, expensive

### Verdict cho VN creator
**Seedance 2.0 cho 80% project.** Kling cho VFX phức tạp. Veo 3 cho global brand campaign cần English text rendering.

---

## 🎯 What Seedance 2.0 is BAD at

Honest list — saves you headaches:

❌ **English text trong video** — chữ tiếng Anh trên billboard, sign sẽ thường lệch chữ. Solution: add text trong post-production (CapCut, AE).

❌ **Western elderly faces** — model lệch về Asian dataset, phương Tây 60+ tuổi đôi khi morph weird. Solution: dùng FLUX 1.1 Pro làm reference image trước.

❌ **Hands close-up** — như mọi AI video, hand anatomy là điểm yếu. Solution: avoid extreme CU on hands trong key shots.

❌ **Long continuous shots > 15s** — drift accumulates. Solution: dùng grid storyboard method (8-12s = sweet spot).

❌ **Specific real-world locations** — không identify được "Cầu Vàng Đà Nẵng" specific. Solution: prompt mô tả features ("golden bridge held by giant stone hands").

❌ **Branded products** — không recreate Coca-Cola can chính xác. Solution: tạo generic version, brand sau trong post.

---

## 📈 Version History

| Version | Released | Key features |
|---------|:--------:|--------------|
| Seedance 1.0 | Q4 2024 | Initial T2V release |
| Seedance 1.5 | Q2 2025 | Image-to-video added |
| Seedance 2.0 | Q4 2025 | Major quality jump, character consistency |
| Seedance 2.1 | April 2026 | Audio generation, camera control |
| Seedance 2.2 | (rumored mid-2026) | Multi-shot continuity |

---

## 💰 Pricing (May 2026)

### On Jimeng / Dreamina (with VPN)
- 480p Fast: 30-50 credits/video (~$0.30-0.50)
- 1080p Standard: 150-250 credits/video (~$1.50-2.50)
- 4K Pro: 400+ credits/video (~$4+)
- Daily free tier: 50-100 credits

### On 0ai.vn (Vietnam direct)
- Subscription model: 200K-500K VND/tháng
- Pay-per-render available
- Support 4K + audio
- Có chatbot tiếng Việt support

### On API (Volcengine / ByteDance Cloud)
- $0.50-1.50/video for 480p
- $2-4/video for 1080p
- Higher latency but unlimited generations

---

## 🚀 Getting Started

### Path 1: Quick test (5 phút)
1. Vào [0ai.vn](https://0ai.vn) — không cần VPN
2. Sign up (free trial)
3. Upload 1 ảnh tham chiếu
4. Prompt đơn giản: "Camera slowly pushes in on the subject"
5. Generate 480p Fast → xem kết quả

### Path 2: Full production setup (1 ngày)
1. Đọc [The 6-Step Prompt Formula](02-six-step-formula.md)
2. Đọc [3-Layer Motion Prompt Structure](03-three-layer-prompt.md)
3. Đọc [Storyboard Grid Method](04-grid-method.md)
4. Build first project theo [9-Panel Workflow](../workflows/01-grid-9-panel.md)
5. Iterate

---

## 📚 Next Reading

- [02 — The 6-Step Prompt Formula](02-six-step-formula.md) — Foundation
- [03 — 3-Layer Motion Prompt](03-three-layer-prompt.md) — 2026 standard
- [04 — Storyboard Grid Method](04-grid-method.md) — Save 70% credits
- [06 — Platforms Comparison](06-platforms-comparison.md) — Jimeng vs 0ai.vn

---

[← Resources](README.md) · [Main README](../README.md)
