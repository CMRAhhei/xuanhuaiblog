---
title: "hugo的备忘录"
date: 2025-12-24T11:50:00+08:00  # 必须有横杠，建议加上具体时间
draft: false                     # 确保不是草稿，否则归档页可能抓取不到
---

### 📝 关于 Hugo 的日常使用

* **新建**：使用命令 `hugo new posts/my-new-post.md`。这样 Hugo 会自动带上日期。
* **编写**：在 VS Code 里编写 Markdown，建议安装 `Markdown All in One` 插件。
* **管理**：修改特殊页面，路径如下：
    * 关于页面：`content/about.md`
    * 友链页面：`content/friend.md`

---

### 🛠️ 本地调试 SOP
1.  **启动服务**：养成运行 `hugo server -D` 的习惯。
2.  **实时预览**：在浏览器访问 `http://localhost:1313`。
3.  **验收检查**：确认头像、图片、排版无误后再提交。

---

### 🚀 云端同步（自动化生产线）
由于已接通 Vercel，维护动作只需三步：
1. `git add .`
2. `git commit -m "Update: 添加关于电气的备忘录"`
3. `git push`

> **提示**：一旦 push 成功，Vercel 会自动构建并刷新域名内容。