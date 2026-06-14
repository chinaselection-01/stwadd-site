# STWADD Website

这是 STWADD（永康市思特瓦德家居用品有限公司）的企业官网，基于 petmanufacturer.com 的设计风格重建。

## 🌐 网站

- 原站：https://www.stwadd.com
- 新站：本地预览后可部署到 GitHub Pages / Vercel / Netlify

## 📁 文件结构

```
stwadd-site/
├── index.html          # 首页
├── about.html          # 关于我们
├── contact.html        # 联系我们
├── css/
│   └── style.css       # 主样式文件
├── js/                 # JavaScript（待添加）
├── images/             # 本地图片（可选）
├── products.yml        # 📦 产品数据（核心！）
└── README.md           # 本文件
```

## 📦 如何通过 GitHub 添加/修改产品

### 方法一：直接编辑 products.yml

1. 打开 GitHub 仓库
2. 找到 `products.yml` 文件
3. 点击编辑（✏️ 图标）
4. 按格式添加新产品：
```yaml
- name: "产品名称"
  category: "产品分类"
  link: "产品详情页链接"
  image: "产品图片URL"
  description: "产品简短描述"
```
5. Commit changes → 网站自动更新

### 方法二：本地编辑后 Push

```bash
# 1. 编辑 products.yml 添加新产品
# 2. 提交到 GitHub
git add .
git commit -m "添加新产品: XXX"
git push
```

## 🔧 网站修改指南

### 修改公司信息
编辑 `index.html` / `about.html` / `contact.html` 中的相关文字

### 修改联系方式
搜索替换以下信息：
- 电话：`+86 150 8822 8843`
- 邮箱：`bob@stwadd.com`
- WhatsApp：`8615088228843`
- 地址：`No.8 Qianjin Industrial Zone, Yongkang City, Zhejiang Province, China`

### 修改配色
编辑 `css/style.css` 中的 CSS 变量：
- `--primary: #FF6B35` — 主色调（橙色）
- `--secondary: #1A2B4A` — 次要色（深蓝）

## 🔗 保留的原始链接

以下链接指向原站 stwadd.com，已保留以维持 SEO 流量：

- 产品分类页：`/stainless-steel-tumbler.html` 等
- 产品详情页：各产品独立链接
- 新闻页：`/news.html`
- 服务页：`/services.html`
- 视频页：`/video.html`
- 隐私政策：`/doc/privacy-policy.html`
- 图片资源：`https://img.yfisher.com/m5671/...`

## 📋 待办

- [ ] 替换产品图片为实际产品图片（当前使用 banner 占位图）
- [ ] 配置 GitHub Pages 自动部署
- [ ] 添加更多产品页面
- [ ] 设置表单提交后端（Formspree / 自建API）
- [ ] 添加 Google Analytics
- [ ] 优化 SEO meta 标签
