# SaltLine — Fable 5.2 FPS

一款小巧的浏览器第一人称射击游戏：场景设定在一个雨天的集装箱港口，只有一个关卡。你需要切断三个上行链路中继，同时躲避无人机（“海鸥”）和机器狗（“猎犬”）的追捕。

<img width="1685" height="906" alt="image" src="https://github.com/user-attachments/assets/8dd32149-90f4-4d69-a573-4411a49a9ba9" />

## 演示

https://realcodebear.github.io/saltline-fable-5.2/

## 出处

- 由 **Claude Fable 5.2** 开发。该运行由 Felix Rieseberg (Anthropic) 设置，并于 2026 年 11 月 9 日在 X 上分享：

https://x.com/felixrieseberg/status/2119925633564463609

- 原始可玩版本：https://claude.ai/artifact/BGY1SztrAYcJQHSsnHHGmp

- 根据他的帖子：一个提示，无人为反馈，运行时间约 8 小时，约 270 万个输出令牌和 4.45 亿个输入令牌（大量缓存），按 API 定价计算，成本约为 550 美元。模型、声音和纹理均由代码生成。这些数据是他自己提供的，未经核实。

游戏的所有功劳都归于其原作者。此仓库是镜像仓库，方便用户在本地运行。如果您是作者并希望将其移除，请提交 issue。

## 与原版本相比有哪些变化

游戏代码没有任何改动。 claude.ai 的框架运行时脚本已从 `<head>` 中移除，并添加了文档类型声明 (doctype)、字符集声明 (charset) 和视口声明 (viewport) 标签，使该文件能够作为普通网页运行。

## 运行它

```sh

python3 -m http.server 8731

```

然后打开 http://localhost:8731 并点击页面以捕获鼠标并启动声音。

整个游戏只有一个文件，`index.html`（约 1.4 MB）。它捆绑了 three.js 并从 Google Fonts 加载字体。没有其他外部资源。
