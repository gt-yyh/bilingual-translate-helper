# 双语翻译助手 - AI 网页与视频字幕双语翻译

一个 Tampermonkey 油猴脚本：为网页正文和视频字幕（YouTube、X/Twitter）提供 AI 双语翻译。

- 接口：DeepSeek 官方接口，或任意 OpenAI 兼容接口（可填自定义 Base URL）
- 模式：原文 + 译文双语显示，或仅显示译文
- 视频字幕：YouTube 与 X（Twitter）视频的字幕双语叠加，支持全屏
- 其它：输入框三连空格翻译、悬浮球控制面板、字幕过滤与样式自定义

## 安装

1. 浏览器安装 [Tampermonkey](https://www.tampermonkey.net/) 扩展
2. 安装脚本（最新版）：

   https://raw.githubusercontent.com/gt-yyh/bilingual-translate-helper/main/dist/bilingual-translate-helper.user.js

3. 打开任意网页，用悬浮球或脚本菜单进入设置，填入 API Key 后即可使用

## 自动更新

脚本头部声明了：

```
@updateURL   https://raw.githubusercontent.com/gt-yyh/bilingual-translate-helper/main/dist/bilingual-translate-helper.user.js
@downloadURL https://raw.githubusercontent.com/gt-yyh/bilingual-translate-helper/main/dist/bilingual-translate-helper.user.js
```

`dist/bilingual-translate-helper.user.js` 始终指向最新版本，安装一次后 Tampermonkey 会自动检测更新。

## 目录说明

| 路径 | 说明 |
| --- | --- |
| `dist/bilingual-translate-helper.user.js` | 最新版本（自动更新目标） |
| `dist/bilingual-translate-helper-1.1.0.user.js` | 1.1.0 版本快照 |
| `dist/bilingual-translate-helper-1.0.1.user.js` | 1.0.1 版本快照 |

历史版本也随各 Release 附件提供下载。

## 版本记录

### 1.1.0

- 新增 X（Twitter）视频字幕双语翻译
- 修复全屏/影院模式字幕错位

### 1.0.1

- 首个发布版本：网页双语翻译、YouTube 字幕双语、DeepSeek / OpenAI 兼容接口、三连空格翻译、悬浮球面板

## 许可

MIT
