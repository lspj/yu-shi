# 蓝色大肥鱼表情包 · AstrBot Meme Manager 表情包（自建镜像）

收录 **133 张** 蓝色大肥鱼（DeepSeek 娘 / Whale-chan）表情包，按 **16 个聊天语义分类** 整理，可直接用 AstrBot「表情包管理器」（`meme_manager`）从 GitHub 安装。

> 素材来自公开分享的大肥鱼表情包整理（梗鲸 [aigengtu.com](https://aigengtu.com/) 收录的同系列图片），版权归各位原作者；本仓库只做分类整理与自建镜像，请勿商用。

## 目录结构

```text
.
├── manifest.json        # 表情包清单（id: blue-fat-fish-meme-pack）
├── memes/
│   ├── happy/           # 16 个语义分类，每类若干张图
│   ├── angry/
│   ├── sad/
│   ├── confused/
│   ├── surprised/
│   ├── shy/
│   ├── sleep/
│   ├── affection/
│   ├── food/
│   ├── money/
│   ├── greeting/
│   ├── work/
│   ├── entertainment/
│   ├── teasing/
│   ├── reply/
│   └── portrait/
└── previews/
    └── cover.jpg
```

分类说明写在 `manifest.json` 的 `categories` 字段里，表情包管理器会把这些描述写进提示词，让模型按语境挑图。

## 在 AstrBot 里安装

1. 打开 AstrBot 后台 → **插件 → 表情包管理器**（`meme_manager`）。
2. 进入 **资源广场**，切到 **从 GitHub 安装（使用自定义来源）**。
3. 填写：

   | 字段 | 值 |
   | --- | --- |
   | 仓库 | `lspj/yu-shi` |
   | 分支 / 标签 / 提交 | `main` |
   | 子目录 | `.` |

4. 点安装；装好后到 **设置中心 → 使用规则** 把「蓝色大肥鱼表情包」设为默认或绑定到指定会话 / 人格。

也可以直接用「表情包管理器」的资源包更新功能，从本仓库拉取新版本。

## 分类一览

| 分类 | 张数 | 适用场景 |
| --- | --- | --- |
| happy | 9 | 开心、庆祝、夸奖 |
| angry | 16 | 生气、责备、不耐烦、夸张威胁 |
| sad | 5 | 委屈、难过、被打击 |
| confused | 9 | 看不懂、疑问、发呆 |
| surprised | 5 | 惊吓、震惊、紧张 |
| shy | 3 | 害羞、脸红、被夸 |
| sleep | 4 | 困、晚安、休息 |
| affection | 8 | 比心、亲亲、送礼、安慰 |
| food | 12 | 吃饭、干饭、要饭 |
| money | 8 | token、充值、要钱、炫富 |
| greeting | 6 | 打招呼、冒泡、登场 |
| work | 8 | 干活、打字、跑数据、摸鱼 |
| entertainment | 10 | 唱歌、游戏、整活、玩梗 |
| teasing | 18 | 吐槽、自嘲、嘴硬、反讽 |
| reply | 5 | 应答、拒绝、安静等直接回应 |
| portrait | 7 | 立绘、形象展示、无明确情绪 |

## 协议

表情包格式遵循 [AstrBot Meme Pack 规范](https://github.com/anka-afk/astrbot-meme-pack-index)（`schema_version: 1`）：`manifest.json` 与 `memes/<分类>/<图片>` 位于包根目录，图片支持 PNG / JPEG / GIF / WebP。

## 许可

仓库内的整理用清单与文档可自由取用；**图片版权归原作者**，原素材许可未指定，本仓库仅作个人分享整理，请勿商用。
