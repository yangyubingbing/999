# 万宁·活力文旅 网站部署说明

## 📁 部署文件

本文件夹包含以下4个HTML文件：
- `index.html` - 主页
- `diary-detail.html` - 探访实录详情页
- `product-detail.html` - 风物档案详情页
- `culture-detail.html` - 文化解码详情页

## ⚠️ 重要提示

### 图片问题解决方案

**问题原因**：网站中使用的在线图片生成API（neeko-copilot.bytedance.net）可能在某些网络环境下无法访问，导致图片显示不出来。

**解决方案**：

#### 方案1：使用本地图片（推荐）

1. 下载稳定的图片素材到 `images/` 文件夹
2. 修改HTML文件中的图片路径

示例修改：
```html
<!-- 将 -->
<img src="https://neeko-copilot.bytedance.net/api/text_to_image?prompt=...">

<!-- 改为 -->
<img src="images/hero-bg.jpg">
```

#### 方案2：使用稳定的免费图床

可以使用以下图床服务：
- Imgur (https://imgur.com)
- SM.MS (https://sm.ms)
- Cloudinary (https://cloudinary.com)
- Unsplash (https://unsplash.com) - 提供免费高质量图片

#### 方案3：使用占位符图片服务

临时使用占位符：
```html
<!-- 使用placeholder.com -->
<img src="https://via.placeholder.com/1920x1080/4A90B8/FFFFFF?text=Wanning+Hero">

<!-- 使用unsplash随机图片 -->
<img src="https://source.unsplash.com/1920x1080/?beach,hainan">
```

## 🚀 GitHub Pages 部署步骤

1. **创建GitHub仓库**
   - 登录GitHub → 点击"+" → "New repository"
   - 命名：`wanning-tourism`
   - 选择Public
   - 点击"Create repository"

2. **上传文件**
   - 点击"uploading an existing file"
   - 将本文件夹中的4个HTML文件拖拽到上传区域
   - 点击"Commit changes"

3. **开启GitHub Pages**
   - 进入仓库 → Settings → Pages
   - Source: "Deploy from a branch"
   - Branch: 选择 `main`
   - 点击"Save"

4. **等待部署**
   - 等待1-2分钟
   - 访问 `https://你的用户名.github.io/wanning-tourism/`

## 🎯 主要功能

- ✅ 首页背景图（需要稳定的图片源）
- ✅ 探访实录板块（带详情页）
- ✅ 风物档案板块（带详情页）
- ✅ 文化解码板块（带详情页）
- ✅ 互动地图（4个点位标注）
- ✅ 管理者模式（访问码：`wanning2025`）
- ✅ 响应式设计
- ✅ 页面平滑滚动
- ✅ 图片画廊功能
- ✅ 内容编辑功能

## 🔧 常见问题

### Q: 图片不显示怎么办？
A: 请参考上面的"图片问题解决方案"，使用本地图片或稳定的图床服务。

### Q: 如何进入管理者模式？
A: 在首页底部或各详情页，点击"管理员入口"按钮，输入访问码 `wanning2025` 即可进入。

### Q: 互动地图为什么不显示？
A: 可能是地图底图加载失败，请检查网络连接或替换为本地图片。

### Q: 页面样式错乱？
A: 尝试强制刷新页面（Ctrl+F5），或清除浏览器缓存。

## 📝 自定义修改

如需修改内容或样式，请直接编辑对应的HTML文件。所有CSS样式和JavaScript代码都已内嵌在HTML中。

### 管理者模式功能
- 上传/删除图片
- 编辑文字内容
- 管理跳转链接
- 编辑互动地图

---

**创建时间**：2026年6月16日
**版本**：v1.0
