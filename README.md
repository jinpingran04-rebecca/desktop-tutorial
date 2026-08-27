# LOEWE 归处有形 · 小程序交互原型

这是一个纯前端的静态 HTML 交互原型（单文件，无需构建、无需依赖），用于展示 LOEWE「归处有形 Give Home a Form」项目的小程序核心流程与页面设计。

在线预览：部署到 GitHub Pages 后，通过 `https://<你的用户名>.github.io/<仓库名>/` 访问。

## 目录结构

```
.
├── index.html   # 唯一文件，包含全部 HTML / CSS / JS，无外部依赖
└── README.md
```

## 本地预览

无需安装任何东西，直接用浏览器打开 `index.html` 即可，或者在本地起一个静态服务器：

```bash
# 任选其一
python3 -m http.server 8000
# 然后浏览器打开 http://localhost:8000
```

## 部署到 GitHub Pages（推荐，免费、几分钟搞定）

1. 在 GitHub 上新建一个仓库（Public），例如叫 `loewe-prototype`。
2. 把本文件夹里的 `index.html`（和这份 `README.md`）上传到仓库根目录：
   - 网页端操作：进入仓库 → **Add file → Upload files** → 把 `index.html` 拖进去 → **Commit changes**
   - 或命令行操作：
     ```bash
     git init
     git add index.html README.md
     git commit -m "add prototype"
     git branch -M main
     git remote add origin https://github.com/<你的用户名>/<仓库名>.git
     git push -u origin main
     ```
3. 进入仓库 **Settings → Pages**。
4. 在 **Build and deployment** 下，Source 选择 **Deploy from a branch**，Branch 选择 **main**，文件夹选择 **/(root)**，点击 **Save**。
5. 等待 1–2 分钟，页面顶部会出现一个绿色提示和访问链接，形如：
   `https://<你的用户名>.github.io/<仓库名>/`
   打开即可看到原型，可以直接发给评委或同学在手机/电脑浏览器里点击体验。

## 使用说明

- 这是点击跳转型的交互 demo，不是真正的微信小程序（无法在微信里直接打开），仅用于演示页面结构、视觉风格与核心流程逻辑。
- 建议用手机浏览器打开体验最接近真实效果；电脑浏览器打开会看到一个模拟手机边框的画面。
- 页面右下角/底部导航可点击切换 首页 / 社区 / 定制 / 工坊 / 我的 五个板块，返回按钮已实现真实的浏览历史回退。
