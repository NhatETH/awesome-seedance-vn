# ⚖️ Ethics & Law — Vietnam AI Deepfake Regulations 2026

> **AI video creator phải biết.** Luật mới VN về deepfake (hiệu lực 1/1/2026) có penalty từ **50-200 triệu VND** cho misuse. Đây là quick guide không phải legal advice.

[← Back to resources](README.md)

> ⚠️ **Disclaimer:** Nội dung dưới đây là tổng hợp public info. **Không phải legal advice.** Trước khi commercial production, **consult lawyer** chuyên về IP/digital media VN.

---

## 🇻🇳 Tóm tắt 30 giây

### Cấm làm
1. Tạo deepfake **không có sự đồng ý** của người trong video
2. Tạo content **gây hại** đến uy tín, nhân phẩm người khác
3. Tạo content **lừa đảo** (CEO fraud, voice cloning scam)
4. Sử dụng **face minor** (< 18 tuổi) trong content NSFW
5. Recreate **brand assets** chính xác (logo, sản phẩm có trademark)

### Phải làm
1. **Watermark** content AI-generated rõ ràng (nhãn "AI-generated")
2. **Có hợp đồng written** với người xuất hiện trong content
3. **Disclose** AI generation trên platforms (TikTok, YouTube đều require)
4. **Ghi rõ** trong contract với client là AI work
5. **Backup** prompts + generation logs cho compliance audit

### Penalty range
- Vi phạm cá nhân: **5-50 triệu VND**
- Vi phạm thương mại: **50-200 triệu VND**
- Vi phạm gây thiệt hại lớn: **truy cứu hình sự** + bồi thường dân sự

---

## 📜 Văn bản pháp lý chính

### Luật An ninh mạng 2018 (sửa đổi 2024)
- Điều 16: nội dung "trái pháp luật" trên không gian mạng
- Áp dụng cho deepfake gây hại danh dự

### Nghị định 53/2022 (Bảo vệ dữ liệu cá nhân)
- Yêu cầu sự đồng ý của data subject (người trong video)
- Phải có data processing agreement
- Phải xoá data khi yêu cầu

### Nghị định AI 2026 (mới)
- Hiệu lực 1/1/2026
- Định nghĩa "AI-generated content"
- Yêu cầu watermark + disclosure
- Penalty 50-200tr cho vi phạm thương mại

### Luật Sở hữu trí tuệ 2022
- AI-generated content: ai sở hữu? (chưa rõ ràng)
- Recreate brand asset = vi phạm trademark
- Recreate copyrighted character = vi phạm copyright

---

## ✅ Best Practices (Production-Ready)

### Khi tạo content có người thật

**TÔI ĐANG DÙNG ẢNH NGƯỜI THẬT (henshin, face swap):**

✅ **Always:**
- Có **written consent** từ người đó (form trong [Tài liệu pháp lý](#tài-liệu-pháp-lý))
- Specify scope: "for [project name], distribution on [platforms]"
- Giới hạn thời gian: "consent valid for [X] months/years"
- Compensation rõ ràng (free or paid)

❌ **Never:**
- Dùng ảnh người nổi tiếng không có deal
- Dùng ảnh minor (< 18 tuổi) không có parental consent + scope NSFW
- Dùng ảnh ex / ai khác mà họ không biết

### Khi tạo content brand / commercial

**TÔI ĐANG LÀM TVC CHO CLIENT:**

✅ **Always:**
- Contract specify "AI-generated production"
- Client owns final video (or per agreement)
- You retain prompts/process docs (or per agreement)
- Disclose AI usage to platforms (required by TikTok, YouTube, Meta)

❌ **Never:**
- Recreate competitor's branded asset (Apple logo, Nike swoosh, etc.)
- Pass off AI work as "shot on camera" without disclosure
- Sell exclusive rights to prompts you'll reuse

### Khi tạo content cổ trang / lịch sử

✅ **Always:**
- Generic characters (không recreate người thật như Trần Hưng Đạo)
- Era-accurate research (avoid anachronism that misleads)
- Disclaimer: "Reimagined dramatization" if narrative

❌ **Never:**
- Make content claiming to be "real footage from [year]"
- Misrepresent historical figures' actions/words
- Use modern political figures' faces

### Khi tạo content NSFW / mature

⚠️ **NSFW content cần extra care:**

✅ **Required:**
- Platform restrictions (no minor faces ever)
- Age verification of distribution
- Disclose AI nature mandatory
- Comply với VN content rating regulations
- KHÔNG distribute trên TikTok / IG (against TOS)

❌ **NEVER:**
- Use real person face without explicit NSFW consent
- Use minor face EVER (criminal liability)
- Distribute on platforms not allowing NSFW

---

## 🌍 International Considerations

Nếu client là international hoặc distribute ngoài VN:

### EU (GDPR + AI Act 2024)
- Stricter consent requirements
- Right to erasure
- AI Act mandates labeling
- Higher penalties (up to 4% global revenue)

### US (state-level patchwork)
- California: AB-602 deepfake porn law
- Texas: SB-751 election deepfake
- Federal proposed but not passed yet

### China (already strict)
- Real-name verification required
- Deepfake illegal without consent
- Watermark mandatory

### Best practice
Default to strictest jurisdiction (EU rules), saves headaches.

---

## 📋 Compliance Checklist for Every Project

Before publishing, verify:

- [ ] All real people in video have signed consent
- [ ] Consent specifies exact use case + platforms + duration
- [ ] No minor faces unless parental consent + appropriate context
- [ ] No branded assets recreated without authorization
- [ ] No misinformation / political deepfake
- [ ] AI disclosure added to video metadata
- [ ] Watermark "AI-generated" visible (subtle is OK)
- [ ] Prompts + logs backed up (for compliance audit)
- [ ] Client contract specifies AI nature
- [ ] Platform-specific disclosure done (TikTok AI label, etc.)

---

## 📝 Tài liệu pháp lý — Templates

### Consent Form (VN — for real person in AI video)

```
PHIẾU ĐỒNG Ý SỬ DỤNG HÌNH ẢNH AI

Tôi, [TÊN NGƯỜI XUẤT HIỆN], CCCD/CMND số [...], 
đồng ý cho [TÊN CREATOR/AGENCY] sử dụng hình ảnh của tôi 
trong sản phẩm AI-generated video với các điều kiện:

1. PHẠM VI: [Mô tả cụ thể project, platform, thời lượng]
2. THỜI GIAN HIỆU LỰC: từ [ngày] đến [ngày]
3. PLATFORM: [TikTok, YouTube, IG, web client X]
4. KHÔNG ĐƯỢC: [list các use case bị cấm — chính trị, NSFW, etc.]
5. THÙ LAO: [free / số tiền cụ thể]

Tôi hiểu rằng sản phẩm AI-generated có thể không hoàn toàn 
giống tôi và đồng ý với điều này.

Ký tên: [...] Ngày: [...]
```

### Client Contract Clause (for AI-generated work)

```
ĐIỀU KHOẢN CÔNG NGHỆ AI:

Bên A (Creator/Agency) xác nhận sản phẩm video được tạo 
một phần hoặc hoàn toàn bằng AI generation tools 
(Seedance 2.0, GPT Image 2, etc.).

Bên B (Client) hiểu và chấp nhận:
1. Output có thể có biến thể giữa các lần generation
2. Một số chi tiết có thể không 100% theo brief
3. AI disclosure required theo luật VN 2026

Quyền sở hữu:
- Final video: [Bên A / Bên B / shared per agreement]
- Source prompts: [Bên A / Bên B / shared per agreement]
- Underlying AI models: thuộc về creator của model
```

---

## 🆘 Khi có sự cố

### Nếu bị tố vi phạm
1. **DON'T panic, DON'T delete evidence**
2. Contact lawyer chuyên về IP digital media VN
3. Backup tất cả prompts, logs, contracts
4. Document timeline of creation

### Nếu phát hiện ai vi phạm work của bạn
1. Document evidence (screenshots, links)
2. DMCA takedown trên platforms (YouTube, TikTok đều có process)
3. Cease & desist letter qua lawyer
4. Civil lawsuit nếu thiệt hại lớn

---

## 📚 Resources & Further Reading

### Legal references
- Luật An ninh mạng 2018 (sửa đổi 2024)
- Nghị định 53/2022/NĐ-CP
- Luật SHTT 2022
- (Nghị định AI 2026 — link khi public)

### Lawyer / consultant directories VN
- VBOI (Vietnam Bar Association)
- Law firms specializing in digital media: search "luật sư truyền thông số Việt Nam"

### International AI law trackers
- Future of Privacy Forum
- Lawfare AI Law Tracker
- DeepDive AI Policy Newsletter

---

## ⚠️ Final Warning

**Đây không phải legal advice.** Luật thay đổi nhanh, đặc biệt AI law. Trước khi:
- Launch commercial product
- Sign contract lớn (>50tr)
- Use real person face
- Distribute internationally

→ **Consult qualified lawyer.** Không tốn nhiều ($200-500/tư vấn), tránh được rủi ro lớn.

---

[← Resources](README.md) · [Main README](../README.md)
