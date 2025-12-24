---
title: "hugo的备忘录"
date: 2025-12-24
draft: true
---

 ### 关于hugo的使用
新建：使用命令 hugo new posts/my-new-post.md。这样 Hugo 会自动带上日期。
编写：在 VS Code 里写 Markdown。
管理：如果要修改关于页面或友链，去 content/about.md 或 content/friend.md 修改。
本地调试
养成先运行 hugo server -D 的习惯。
在浏览器查看 localhost:1313，确认头像、图片、排版没问题再提交。
### 云端同步（自动化生产线）
由于你接通了 Vercel，你的维护动作只需要：
git add .
git commit -m "Update: 添加关于电气的备忘录"
git push
一旦 push 成功，Vercel 会自动帮你构建并刷新域名内容。