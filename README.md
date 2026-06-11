# salary-cat-lyrics

月薪喵歌词版 — 基于 [qxz4188/salary-cat-web](https://github.com/qxz4188/salary-cat-web) 的增强版本。

## ✨ 新增功能

- 🎶 **歌词动画** — 纯 CSS 实现的逐句淡入淡出歌词效果，模拟歌词滚动
- 🌙 **深色主题** — 暗蓝渐变背景 + 金色歌词，氛围感拉满
- 🎵 **音乐控制** — 右下角浮动按钮，播放/暂停切换
- 🎯 **开屏交互** — 点击启动（兼容浏览器自动播放限制）
- 📦 **单文件版本** — `standalone.html` 内嵌 GIF，无需额外文件

## 📂 文件说明

| 文件 | 说明 |
|------|------|
| `lyrics.html` | 歌词版（需要同目录下的 cat.GIF 和 music.mp3） |
| `standalone.html` | 单文件版（GIF 内嵌 base64，无需额外文件） |
| `embed-notice.html` | 公告嵌入版（透明背景，纯 CSS 歌词动画，适合嵌入其他页面） |

## 🚀 使用

### 方式一：完整版（含音乐）
```bash
git clone https://github.com/qxz4188/salary-cat-web.git
# 将 lyrics.html 放入项目目录，替换 index.html 或单独打开
```

### 方式二：单文件版
直接浏览器打开 `standalone.html` 即可。

### 方式三：嵌入公告/网页
将 `embed-notice.html` 的内容粘贴到支持 HTML 的公告框中。

## 🎨 自定义歌词

编辑 HTML 中的 `<span>` 标签即可，每行一句：

```html
<div class="lyrics">
  <span>你的第一句歌词</span>
  <span>你的第二句歌词</span>
  ...
</div>
```

调整速度：修改 CSS 中的 `animation-delay` 和 `@keyframes showLine` 的总时长。

## 📋 原版 vs 歌词版

| 特性 | 原版 | 歌词版 |
|------|------|--------|
| 猫咪动画 | ✅ | ✅ |
| 背景音乐 | ✅ | ✅ |
| 歌词动画 | ❌ | ✅ |
| 深色主题 | ✅ | ✅ 增强 |
| 音乐控制按钮 | ❌ | ✅ |
| 单文件部署 | ❌ | ✅ |
| 嵌入公告 | ❌ | ✅ |

## 📄 License

MIT

## 🙏 致谢

- [qxz4188/salary-cat-web](https://github.com/qxz4188/salary-cat-web) — 原始项目
