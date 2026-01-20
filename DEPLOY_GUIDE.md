# 不依赖电脑运行 Neo Tarot 的方案

Neo Tarot 是纯前端应用，可以部署到免费的静态网站托管服务上，彻底摆脱对本地电脑的依赖。

## 🎯 推荐方案：部署到免费托管平台

### 1. GitHub Pages（推荐）

**优点：**
- 完全免费
- 无需任何配置
- 自动 HTTPS
- 支持自定义域名

**部署步骤：**

```bash
# 1. 克隆仓库
git clone https://github.com/hqzzdsda/neo-tarot.git
cd neo-tarot

# 2. 创建 GitHub 仓库
# 访问 https://github.com/new 创建一个新仓库

# 3. 关联并推送
git remote add origin https://github.com/您的用户名/您的仓库名.git
git branch -M main
git push -u origin main

# 4. 启用 GitHub Pages
# 进入仓库设置 → Pages → 选择 main 分支 → 保存
# 等待几分钟，访问 https://您的用户名.github.io/您的仓库名/
```

### 2. Vercel

**优点：**
- 免费计划
- 全球 CDN，速度快
- 一键部署

**部署步骤：**
1. 访问 https://vercel.com/
2. 使用 GitHub 账号登录
3. 点击 "New Project"
4. 选择您的仓库
5. 点击 "Deploy"
6. 等待部署完成，访问生成的域名

### 3. Netlify

**优点：**
- 免费计划
- 支持自动部署
- 自定义域名

**部署步骤：**
1. 访问 https://www.netlify.com/
2. 使用 GitHub 账号登录
3. 点击 "Add new site" → "Import an existing project"
4. 选择您的仓库
5. 点击 "Deploy site"
6. 等待部署完成，访问生成的域名

## 📱 移动设备本地运行方案

### iOS 设备

1. **下载应用文件**：
   - 将项目文件下载到电脑
   - 通过 AirDrop 发送到 iOS 设备

2. **使用离线浏览器**：
   - 下载 "Offline Browser" 应用
   - 导入项目文件夹
   - 打开 index.html

### Android 设备

1. **下载应用文件**：
   - 将项目文件下载到手机存储

2. **使用本地文件浏览器**：
   - 下载支持本地 HTML 的浏览器（如 Firefox、Kiwi Browser）
   - 定位到 index.html 文件
   - 点击打开

## 🚀 部署注意事项

1. **API Key 保护**：
   - 当前代码中 API Key 是客户端暴露的，建议在部署时设置使用自己的 API Key
   - 修改 `script.js` 中的 `API_KEY` 变量

2. **摄像头功能**：
   - 部署后，摄像头功能需要用户授权
   - 确保使用 HTTPS 协议

3. **更新维护**：
   - GitHub Pages：推送更新后自动部署
   - Vercel/Netlify：可以设置自动部署

## 🌟 部署后的使用

部署完成后，您可以：
- 在任何有网络的地方访问应用
- 分享链接给朋友
- 在手机、平板、电脑上随时使用
- 不再依赖本地电脑运行

这样您就可以彻底摆脱电脑和距离的限制，随时随地享受 Neo Tarot 的神秘体验了！✨