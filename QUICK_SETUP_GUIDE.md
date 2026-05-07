# 🚀 Quick Setup Guide — Đọc file này TRƯỚC TIÊN

> Hướng dẫn từ A-Z để đưa repo này lên GitHub trong 30 phút.

---

## 📋 Trước khi bắt đầu

Bạn cần:
- ✅ Tài khoản GitHub (miễn phí)
- ✅ Git cài đặt trên máy ([download](https://git-scm.com/))
- ✅ Editor (VS Code khuyên dùng)
- ✅ 30 phút thời gian

---

## ⚡ Setup trong 30 phút

### Bước 1 — Customize repo (10 phút)

Mở repo trong VS Code. Repo đã được customize sẵn cho `@0ailab` — chỉ cần thay GitHub username nếu khác.

**Cách làm trong VS Code:**
1. Cmd/Ctrl + Shift + F (Find in Files)
2. Tìm `NhatETH` → Replace All với GitHub username của bạn (nếu khác)

**Files cần check kỹ:**
- `README.md`
- `README.en.md`
- `CONTRIBUTING.md`
- `community/showcase.md`

---

### Bước 2 — Tạo GitHub Repo (5 phút)

1. Vào [github.com/new](https://github.com/new)
2. Repository name: `awesome-seedance-vn`
3. Description: `🎬 Awesome Seedance 2.0 + GPT Image 2 — Vietnamese-English bilingual resource`
4. Public ✅
5. **KHÔNG** check "Add README" / "Add .gitignore" / "Add license"
6. Create repository

---

### Bước 3 — Push code lên (5 phút)

Mở terminal trong thư mục `github_repo/`:

```bash
cd /path/to/github_repo
git init
git add .
git commit -m "Initial launch — bilingual VN/EN, prompts library, guides"
git branch -M main
git remote add origin https://github.com/NhatETH/awesome-seedance-vn.git
git push -u origin main
```

---

### Bước 4 — Setup repo settings (5 phút)

Vào GitHub → Repo settings:

#### About (cột phải README)
- **Description:** `🎬 Vietnamese-English bilingual resource for Seedance 2.0 + GPT Image 2 (2026 trends)`
- **Website:** https://x.com/0ailab
- **Topics:** `seedance` `seedance-2` `gpt-image-2` `ai-video` `vietnamese` `prompts` `storyboard-grid` `awesome-list`

#### Settings → General
- ✅ **Allow squash merging**
- ✅ **Allow rebase merging**
- ❌ Disable "Allow merge commits" (cleaner history)

---

## 🎉 Đã xong! Giờ làm gì tiếp?

### Ngày 1 (hôm nay)
- [ ] Post launch tweet thread trên [@0ailab](https://x.com/0ailab)
- [ ] Share repo trong cộng đồng Zalo: [Tham gia](https://zalo.me/g/caqqva644)
- [ ] Add 3 prompts còn thiếu cho 50 prompts MVP

### Tuần 1
- [ ] DM 10 friends ask for star + feedback
- [ ] Post lên 3 community VN
- [ ] Reply tất cả issues / PRs đầu tiên

### Tuần 2-12
- [ ] Follow [Launch Playbook](community/internal-launch-playbook.md)

---

## 📝 Launch Tweet Thread Template

Copy paste, customize, post từ [@0ailab](https://x.com/0ailab):

```
🚀 LAUNCHING: Awesome Seedance VN

Cộng đồng AI video tiếng Việt đầu tiên về Seedance 2.0 + GPT Image 2.

Tất cả tài liệu mình đã build & test trong 6 tháng qua.
Mở source code, miễn phí cho cộng đồng.

🧵👇
[1/10]
```

```
[2/10] Có gì trong repo?
🛍️ Affiliate / TikTok prompts
🎭 Drama short prompts
📺 TVC sản phẩm prompts
🎵 Music Video prompts
🌏 Documentary prompts

Tất cả đã test. Tất cả song ngữ VN+EN.
```

```
[3/10] 5 trending viral formats Q2/2026:
🌟 Henshin transformation
🌀 Satisfying Loop
👁️ POV / Orb 15s
🧴 ASMR Macro
🌳 What-If Surreal

View potential: 100K-2M+ per clip
```

```
[4/10] Deep-dive guides về:
- 3-Layer Motion Prompt (NEW 2026 standard)
- Storyboard Grid Method (save 70% credits)
- Scene Archetype Router
- Bảng giá thị trường VN (data thật!)
```

```
[5/10] Tại sao tập trung VN?

Tài liệu EN về Seedance đã nhiều rồi. Cộng đồng VN lại thiếu.
Repo này localize tất cả:
- Văn hoá VN (áo dài, Hội An, Saigon)
- Bảng giá VN (data từ 15+ agency)
- Tuân thủ luật deepfake VN
```

```
[6/10] Pipeline 4 bước CHUẨN 2026:

1. ChatGPT → kịch bản tiếng Việt
2. GPT Image 2 → grid 3×3 storyboard
3. Claude → motion prompt 3-layer
4. Seedance → video 8-15s

Tiết kiệm 60-70% credits vs old T2V.
```

```
[7/10] System prompts free để paste:

🤖 Claude Director V2
🤖 ChatGPT Storyboard Designer

Set một lần → generate prompts tự động.
```

```
[8/10] Real case studies từ VN:

💄 Beauty: 1.5tr/clip ASMR
🏠 Real estate: 15-30tr/walkthrough
🎵 K-pop MV: 5-30tr per piece

Full ROI breakdown cho mỗi case.
```

```
[9/10] Repo focus 2 nền tảng video:
🇨🇳 Jimeng (cần VPN, nhiều quota free)
🇻🇳 0ai.vn (direct, không cần VPN, 4K)

+ ChatGPT cho storyboard
+ Claude cho motion prompt
```

```
[10/10] ⭐ Star: github.com/NhatETH/awesome-seedance-vn
💬 Cộng đồng Zalo: zalo.me/g/caqqva644

PRs welcome. Bilingual contributions appreciated.

Cùng build cộng đồng VN AI video 🚀
```

---

## ⚠️ Common Mistakes to Avoid

### 1. Push tất cả files một lượt
**Đúng:** Test internal links trước

### 2. Promote quá hung hăng day 1
**Đúng:** Soft launch → friends → feedback → polish → bigger launch tuần 2

### 3. Forget update CHANGELOG
**Đúng:** Mỗi PR phải có entry CHANGELOG (or update it batch-style cuối tuần)

### 4. Quên add .gitignore
**Đúng:** Đã có rồi! Check nó cover các sensitive files

---

## 💰 Monetization Ideas (Phase 2)

Sau khi có 200-500 stars (Tuần 4-8):

### Free → Premium ladder
1. **Free:** Repo + Zalo community + basic guides
2. **Tier 1 (99K/tháng):** Member-only tier + early access
3. **Tier 2 (499K/lần):** Pro Pack course (advanced prompts + case studies)
4. **Tier 3 (1.5tr/giờ):** 1-on-1 consulting

### Affiliate revenue
- 0ai.vn affiliate (5-10%)

### Sponsorship
- AI tool companies pay for "Featured in resources" mention
- 3-10tr/tháng per sponsor

### Course business
- 1-3tr/student
- Target 20-50 students/cohort
- 4 cohorts/year = 60-200 triệu/năm

---

## ✅ Final Checklist

Trước khi go-live:

- [ ] Repository pushed to GitHub
- [ ] About section filled (description, topics, website)
- [ ] At least 30 prompts in repo
- [ ] At least 5 guides in resources/
- [ ] Cộng đồng Zalo link hoạt động
- [ ] X account [@0ailab](https://x.com/0ailab) sẵn sàng
- [ ] Launch tweet thread drafted
- [ ] First 10 friends notified
- [ ] [Launch Playbook](community/internal-launch-playbook.md) bookmarked

---

**🎉 Bạn đã sẵn sàng. Chúc bạn launch thành công và build cộng đồng VN AI video!**

---

**Updated:** 2026-05-07
**Total time investment to launch:** 30 phút setup + 6-10 hrs/tuần để scale
