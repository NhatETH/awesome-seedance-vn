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

Mở repo trong VS Code. Tìm và replace các placeholder sau:

| Placeholder | Replace với |
|-------------|------------|
| `YOUR_USERNAME` | GitHub username của bạn |
| `your_handle` | X (Twitter) handle của bạn |
| `@your_handle` | @ + Twitter handle |
| `your-domain.com` | Domain email của bạn |
| `YOUR_DISCORD_LINK` | Discord invite link (tạo sau) |

**Cách làm trong VS Code:**
1. Cmd/Ctrl + Shift + F (Find in Files)
2. Tìm `YOUR_USERNAME` → Replace All với username
3. Lặp lại với các placeholder khác

**Files cần check kỹ:**
- `README.md` (file quan trọng nhất)
- `README.en.md`
- `CONTRIBUTING.md`
- `CODE_OF_CONDUCT.md`
- `community/showcase.md`

---

### Bước 2 — Tạo GitHub Repo (5 phút)

1. Vào [github.com/new](https://github.com/new)
2. Repository name: `awesome-seedance-vn` (hoặc tên bạn thích)
3. Description: `🎬 Awesome Seedance 2.0 + GPT Image 2 — Vietnamese-English bilingual resource`
4. Public ✅
5. **KHÔNG** check "Add README" / "Add .gitignore" / "Add license" (đã có sẵn)
6. Create repository

---

### Bước 3 — Push code lên (5 phút)

Mở terminal trong thư mục `github_repo/`:

```bash
cd /path/to/github_repo
git init
git add .
git commit -m "Initial launch — bilingual VN/EN, 12 prompts, 5 guides, full structure"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/awesome-seedance-vn.git
git push -u origin main
```

---

### Bước 4 — Setup repo settings (5 phút)

Vào GitHub → Repo settings:

#### About (cột phải README)
- **Description:** `🎬 Vietnamese-English bilingual resource for Seedance 2.0 + GPT Image 2 (2026 trends)`
- **Website:** (link Discord hoặc landing page)
- **Topics:** `seedance` `seedance-2` `gpt-image-2` `ai-video` `vietnamese` `prompts` `storyboard-grid` `awesome-list` `bytedance` `openai`

#### Settings → General
- ✅ **Allow squash merging**
- ✅ **Allow rebase merging**
- ❌ Disable "Allow merge commits" (cleaner history)

#### Settings → Pages (optional but recommended)
- Source: Deploy from branch
- Branch: `main` / Folder: `/ (root)`
- Theme: Slate / Cayman (pick one)
- Custom domain (later)

#### Settings → Branches
- Default branch: `main`
- Add branch protection rule for `main`:
  - Require pull request before merging
  - Require 1 approval (optional, when you have collaborators)

---

### Bước 5 — Tạo Discord (5 phút)

1. Vào [discord.com/new](https://discord.com/) (cần app desktop)
2. Tạo server với template "Project / Friends"
3. Đổi tên: `Awesome Seedance VN`
4. Tạo channels:
   - `#welcome` — read only, intro rules
   - `#announcements` — read only, your updates
   - `#general-discussion` — chat tự do
   - `#prompt-sharing` — share prompts community
   - `#help` — Q&A
   - `#showcase` — share works
   - `#contributors` — for active contributors
   - `#pricing-strategy` — VN business talk
5. Generate **never-expire invite link** → paste vào README.md

---

## 🎉 Đã xong! Giờ làm gì tiếp?

### Ngày 1 (hôm nay)
- [ ] Tạo X account `@SeedanceVN` (hoặc tên bạn)
- [ ] Post launch tweet thread (xem template bên dưới)
- [ ] Add 3 prompts còn thiếu cho 50 prompts MVP

### Tuần 1
- [ ] DM 10 friends ask for star + feedback
- [ ] Post lên 3 community VN
- [ ] Reply tất cả issues / PRs đầu tiên

### Tuần 2-12
- [ ] Follow [Launch Playbook](community/internal-launch-playbook.md)

---

## 📝 Launch Tweet Thread Template

Copy paste, customize, post:

```
🚀 LAUNCHING: Awesome Seedance VN

The first comprehensive Vietnamese-English resource for AI video creation with Seedance 2.0 + GPT Image 2.

What's inside 🧵👇

[1/10]
```

```
[2/10] 50+ ready-to-use prompts:
🛍️ Affiliate / TikTok
🎭 Drama short
📺 TVC sản phẩm
🎵 Music Video
🌏 Documentary

All tested. All bilingual VN+EN.
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
[4/10] 8 deep-dive guides covering:
- 3-Layer Motion Prompt (NEW 2026 standard)
- Storyboard Grid Method (save 70% credits)
- Scene Archetype Router
- Vietnam market pricing (exclusive data!)
```

```
[5/10] Why Vietnamese-focused?

While EN resources for Seedance are abundant, VN community is underserved. We localize everything:
- VN cultural references (áo dài, Hội An, Saigon)
- VN market pricing (real data from 15+ agencies)
- VN deepfake law compliance
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
[7/10] Free system prompts ready to paste:

🤖 Claude Director V2
🤖 ChatGPT Storyboard Designer
🤖 Grok Viral Format Expert

Set once → generate prompts automatically.
```

```
[8/10] Real case studies from VN agencies:

💄 Beauty: 1.5tr/clip ASMR
🏠 Real estate: 15-30tr/walkthrough
🎵 K-pop MV: 5-30tr per piece

Full ROI breakdown for each.
```

```
[9/10] Built on shoulders of giants:

Inspired by @EvoLinkAI, @AtlasCloud, @MrLarus, @Saccc_c, @LudovicCreator, @deredleritt3r, and many more.

Localized for VN market 🇻🇳
```

```
[10/10] ⭐ Star: github.com/YOUR_USERNAME/awesome-seedance-vn
💬 Discord: [your link]
📺 YouTube: [your link]

PRs welcome. Bilingual contributions appreciated.

Let's build the VN AI video community together 🚀
```

---

## ⚠️ Common Mistakes to Avoid

### 1. Push tất cả files một lượt
**Đúng:** Test internal links trước (use `markdown-link-check` action)

### 2. Promote quá hung hăng day 1
**Đúng:** Soft launch → friends → feedback → polish → bigger launch tuần 2

### 3. Forget update CHANGELOG
**Đúng:** Mỗi PR phải có entry CHANGELOG (or update it batch-style cuối tuần)

### 4. Quên add .gitignore
**Đúng:** Đã có rồi! Check nó cover các sensitive files (internal-launch-playbook.md)

### 5. Sử dụng tên/handle giống hệt 1 creator nổi tiếng
**Đúng:** Differentiate. Ví dụ `@SeedanceVN` thay vì `@Seedance` (đã có).

---

## 💰 Monetization Ideas (Phase 2)

Sau khi có 200-500 stars (Tuần 4-8):

### Free → Premium ladder
1. **Free:** Repo + Discord + basic guides
2. **Tier 1 (99K/tháng):** Member-only Discord channel + early access
3. **Tier 2 (499K/lần):** Pro Pack course (20 advanced prompts + 5 case studies)
4. **Tier 3 (1.5tr/giờ):** 1-on-1 consulting

### Affiliate revenue
- 0ai.vn affiliate (5-10%)
- Higgsfield affiliate (program TBD)
- Cyberbara affiliate

### Sponsorship
- AI tool companies pay for "Featured in resources" mention
- 3-10tr/tháng per sponsor

### Course business
- 1-3tr/student
- Target 20-50 students/cohort
- 4 cohorts/year = 60-200 triệu/năm

---

## 📞 Need Help?

Khi gặp vấn đề:
1. Search Stack Overflow / GitHub docs trước
2. Ask in `#help` Discord channel (after setup)
3. DM repo maintainer

---

## ✅ Final Checklist

Trước khi go-live:

- [ ] All `[YOUR_USERNAME]` replaced
- [ ] All `[your_handle]` replaced
- [ ] All `[your-domain.com]` replaced
- [ ] Repository pushed to GitHub
- [ ] About section filled (description, topics, website)
- [ ] At least 30 prompts in repo
- [ ] At least 5 guides in resources/
- [ ] Discord server created + invite link in README
- [ ] X account created
- [ ] Launch tweet thread drafted
- [ ] First 10 friends notified
- [ ] [Launch Playbook](community/internal-launch-playbook.md) bookmarked

---

**🎉 Bạn đã sẵn sàng. Chúc bạn launch thành công và build cộng đồng VN AI video!**

---

**Updated:** 2026-05-07
**Total time investment to launch:** 30 phút setup + 6-10 hrs/tuần để scale
