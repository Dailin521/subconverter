# subconverter URL 生成器

一个纯前端页面，用于把 3X-UI 上游订阅链接转换为 Clash/Mihomo 可订阅的 subconverter URL。

## 使用方法

1. 直接打开 `subconverter_web.html`。
2. 填入“转换器地址”和“上游订阅 URL”。
3. 点击“生成链接”，把输出的 URL 填到 Clash/Mihomo 订阅中。

## 说明

- “转换器地址”是你运行 subconverter 的地址（例如 `http://127.0.0.1:25500` 或 VPS 地址）。
- 支持多个上游订阅：一行一个，或用 `|` 合并。
- 可选填写“外部配置 URL”与“订阅名/文件名”参数。
- “获取并检测”会尝试拉取前几行判断 YAML 标记，若浏览器报错通常是 CORS 限制，可直接在新标签页打开链接验证。

## 示例

```
http://127.0.0.1:25500/sub?target=clash&url=<URLENCODED_UPSTREAM>
```
