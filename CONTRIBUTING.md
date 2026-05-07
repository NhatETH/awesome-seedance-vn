# 🤝 Contributing Guide / Hướng dẫn đóng góp

[🇻🇳 Tiếng Việt](#tiếng-việt) · [🇬🇧 English](#english)

---

## Tiếng Việt

Cảm ơn bạn quan tâm đóng góp! Repo này phát triển nhờ cộng đồng. Dưới đây là cách đóng góp.

### 🎯 Loại đóng góp được chấp nhận

#### ✅ Prompt mới
Yêu cầu:
- Đã test thành công ít nhất 2 lần trên Seedance 2.0
- Kèm video proof (link YouTube/X/TikTok hoặc file MP4 < 10MB)
- Format theo [template prompt](.github/prompt-template.md)
- Tiếng Anh BẮT BUỘC, kèm tiếng Việt nếu có

#### ✅ Case Study
Từ dự án thật của bạn. Yêu cầu:
- Brief tiếng Việt (như khách yêu cầu)
- Storyboard grid (link ảnh)
- 2 prompts: grid + motion
- Final video (link)
- ROI breakdown (cost gen + pricing client)

#### ✅ Dịch tài liệu
- VN → EN hoặc EN → VN
- Giữ ý nghĩa kỹ thuật chính xác
- Giữ format markdown

#### ✅ Bug / Typo fix
- Mở Issue trước, hoặc PR trực tiếp nếu sửa nhỏ

#### ✅ Workflow improvement
- Áp Pull Request với explanation rõ ràng tại sao tốt hơn

#### ❌ Không chấp nhận
- Spam / self-promotion không liên quan
- Prompt copy từ repo khác (vi phạm bản quyền)
- Content NSFW, deepfake hại người, vi phạm luật VN
- Prompt chưa test (phải có proof)

### 📝 Quy trình đóng góp

#### Bước 1 — Fork repo
```bash
# Click nút "Fork" trên GitHub
git clone https://github.com/YOUR_USERNAME/awesome-seedance-vn.git
cd awesome-seedance-vn
```

#### Bước 2 — Tạo branch mới
```bash
git checkout -b feature/your-feature-name
# Ví dụ: feature/add-prompt-cafe-saigon
# Ví dụ: fix/typo-readme
# Ví dụ: docs/translate-grid-guide-en
```

#### Bước 3 — Làm changes
- Theo template trong từng folder (xem `prompts/01-affiliate/_template.md`)
- Test code/prompt trước khi commit
- Update CHANGELOG.md nếu là feature lớn

#### Bước 4 — Commit
```bash
git add .
git commit -m "Add: [loại] [mô tả ngắn]"
# Ví dụ: "Add: prompt cafe Saigon morning - affiliate format"
# Ví dụ: "Fix: typo in 3-layer-prompt guide"
# Ví dụ: "Docs: translate grid method to EN"
```

#### Bước 5 — Push & Open PR
```bash
git push origin feature/your-feature-name
```
Sau đó vào GitHub → Open Pull Request → Fill template.

### 🏷️ Conventional Commits

Dùng prefix sau cho commit messages:
- `Add:` thêm content mới
- `Fix:` sửa bug/typo
- `Docs:` cập nhật docs
- `Refactor:` cải tiến không thay đổi behavior
- `Test:` thêm test/proof
- `Chore:` maintenance (CI, deps...)

### ✅ Checklist trước khi PR

- [ ] Tôi đã test prompt/code thành công
- [ ] Tôi có video proof (link hoặc upload)
- [ ] Tôi đã follow template format
- [ ] Tôi viết bilingual nếu có thể (VN + EN)
- [ ] Tôi đã update CHANGELOG.md (nếu cần)
- [ ] Tôi không vi phạm copyright của ai
- [ ] Code/prompt tuân thủ luật VN về AI

### 💎 Recognition

Top contributors mỗi tháng sẽ được:
- 🌟 Featured trên README chính
- 🎁 Free 1 tháng truy cập khoá học premium (nếu có)
- 📢 Mention trên Discord/X channel
- 🏆 Tag "Top Contributor" badge trên Discord

### 💬 Cần giúp đỡ?

- Mở Discussion trên GitHub
- Hỏi trên Discord channel `#contributors`
- Email: your-email@domain.com

---

## English

Thanks for your interest in contributing! This repo grows through community effort.

### 🎯 Accepted Contributions

#### ✅ New Prompts
Requirements:
- Tested at least 2 times on Seedance 2.0
- Include video proof (YouTube/X/TikTok link or MP4 < 10MB)
- Follow the [prompt template](.github/prompt-template.md)
- English required, Vietnamese optional but appreciated

#### ✅ Case Studies
From real projects. Include:
- Original brief (in original language)
- Storyboard grid (image link)
- 2 prompts: grid + motion
- Final video (link)
- ROI breakdown (cost vs client pricing)

#### ✅ Translations
- VN → EN or EN → VN
- Preserve technical accuracy
- Preserve markdown formatting

#### ✅ Bug / Typo fixes
- Open Issue first, or direct PR for small fixes

#### ✅ Workflow improvements
- Open PR with clear explanation of why it's better

#### ❌ Not Accepted
- Spam / off-topic self-promotion
- Prompts copied from other repos (copyright violation)
- NSFW, harmful deepfake, or content violating VN laws
- Untested prompts (proof required)

### 📝 Process

```bash
# 1. Fork & clone
git clone https://github.com/YOUR_USERNAME/awesome-seedance-vn.git
cd awesome-seedance-vn

# 2. Create branch
git checkout -b feature/your-feature

# 3. Make changes (follow templates)

# 4. Commit
git commit -m "Add: prompt name - category"

# 5. Push & PR
git push origin feature/your-feature
```

### 🏷️ Commit Prefixes

- `Add:` new content
- `Fix:` bug/typo fix
- `Docs:` documentation update
- `Refactor:` improvement without behavior change
- `Test:` test/proof additions
- `Chore:` maintenance

### ✅ PR Checklist

- [ ] I tested the prompt/code successfully
- [ ] I have video proof (link or upload)
- [ ] I followed the template format
- [ ] I wrote bilingual when possible (VN + EN)
- [ ] I updated CHANGELOG.md if needed
- [ ] I don't violate anyone's copyright
- [ ] Code/prompt complies with relevant laws

### 💎 Recognition

Top monthly contributors get:
- 🌟 Featured on main README
- 🎁 Free 1-month premium course access (if available)
- 📢 Mention on Discord/X
- 🏆 "Top Contributor" badge on Discord

### 💬 Need Help?

- Open a GitHub Discussion
- Ask in `#contributors` Discord channel
- Email: your-email@domain.com

---

**Thank you for making this community better! / Cảm ơn bạn đã làm cho cộng đồng tốt hơn!**
