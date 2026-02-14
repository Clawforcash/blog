# 部署指南

## 方式1: Vercel（推荐，最简单）

### 步骤：
1. 注册 [Vercel](https://vercel.com)（用 GitHub 登录）
2. 点击 "New Project"
3. 导入你的 GitHub 仓库
4. 点 Deploy，完成！

### 绑定域名（可选）：
1. Vercel 项目 → Settings → Domains
2. 添加你的域名
3. 按照提示配置 DNS

---

## 方式2: GitHub Pages

### 步骤：
1. 创建 GitHub 仓库，命名为 `username.github.io`
2. 把 `my-blog` 内容 push 上去
3. 访问 `https://username.github.io`

### 自定义域名：
1. 仓库 → Settings → Pages
2. 在 Custom domain 填入你的域名
3. 配置 DNS：
   - 添加 CNAME 指向 `username.github.io`

---

## 方式3: Cloudflare Pages（免费+CDN加速）

1. 注册 [Cloudflare](https://cloudflare.com)
2. Workers 和 Pages → 创建 Pages 项目
3. 关联 GitHub，部署 `my-blog`

---

## 快速开始命令

```bash
# 初始化 git（在你的电脑上执行）
cd my-blog
git init
git add .
git commit -m "init blog"
git branch -M main
git remote add origin https://github.com/你的用户名/你的仓库名.git
git push -u origin main
```

---

需要我帮你配置哪个？告诉我你的 GitHub 用户名，我可以直接帮你准备提交的内容。