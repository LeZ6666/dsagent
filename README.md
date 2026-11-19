# DeepSeek Agent

接入 DeepSeek 最新模型的 PWA 智能助手，装到手机主屏即用。

## 能力

-   **思考模式** — deepseek-flash 原生 
easoning_content，思维链可折叠
-   **联网搜索** — deepseek_web_search + deepseek_read_url，回答带引用
-   **工具调用** — 时间、计算器、笔记（执行在手机本地）
-   **图片理解** — 拍照直接问
-   **多会话** — 本地 IndexedDB 持久化，不经过第三方

## 模型

| 模型 | 说明 |
|------|------|
| deepseek-flash | 1M 上下文、384K 输出、快+便宜，支持图片与联网 |
| deepseek-v4-pro | 更强推理，不支持图片/联网 |

## 使用

1. 浏览器打开此页面
2. Safari（iPhone）→ 分享 → **添加到主屏幕**（Android 同理加入桌面）
3. 手机/桌面 Chrome → 地址栏右侧安装按钮

首次使用需要填入 [DeepSeek API Key](https://platform.deepseek.com/api_keys)。

## 部署

纯静态文件，放到任何 HTTPS 主机即可（GitHub Pages / Cloudflare Pages / Vercel / Netlify 等都行）。需要上传：

- index.html
- manifest.webmanifest
- sw.js
- icons/ 目录

本地调试：
ode serve.mjs 提供静态托管 + 演示 mock 接口。

## 许可

MIT
