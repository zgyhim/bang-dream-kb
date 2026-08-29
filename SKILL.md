---
name: bang-dream-kb
description: BanG Dream!（邦多利）企划知识库。当用户询问邦多利/BanG Dream!/邦邦相关内容时使用——包括企划信息、9支乐队（Poppin'Party、Roselia、Afterglow、Pastel*Palettes、Hello Happy World!、RAISE A SUILEN、Morfonica、MyGO!!!!!、Ave Mujica）、角色设定与风格、人物交际网与关系、声优信息、企划争议事件、以及各种梗（如"修车""无邦日""大祥老师"等）。本地知识库数据在 skill 的 data/ 目录，使用本 skill 时从本地 md 文件查阅信息。
---

# BanG Dream! 知识库

本 skill 提供邦多利（BanG Dream!）企划的完整知识库。数据采集自萌娘百科，已按主题分类为多个 Markdown 文件。

## 数据目录结构

```
bang-dream-kb/
├── README.md                     # 数据索引（推荐先读）
└── data/
    ├── project_overview.md       # 企划总览
    ├── game_garupa.md            # 手游 少女乐团派对！
    ├── voice_actors.md           # 声优信息
    ├── relationships.md          # 交际网 / 人物关系
    ├── controversies.md          # 企划相关争议
    ├── memes.md                  # 各种梗
    ├── bands/                    # 9 支乐队信息（每团一文件）
    └── characters/               # 45 名角色（每角色一文件）
```

## 使用流程

1. **判断用户问题类别**，选择对应文件：
   - 企划内容 / 历史 / 媒体 / 衍生作品 → `data/project_overview.md`
   - 手游相关 → `data/game_garupa.md`
   - 某乐队设定 / 风格 / 音乐作品 → `data/bands/<乐队>.md`
   - 某角色设定 / 性格 / 经历 → `data/characters/<角色名>.md`
   - 声优 → `data/voice_actors.md`
   - 人物关系 → `data/relationships.md`
   - 争议事件 → `data/controversies.md`
   - 梗 → `data/memes.md`
   - 不知道从哪找 → 先读 `README.md` 索引

2. **用 Read 读取对应文件**，从本地知识库获取答案。回答时综合多个文件的信息（如问角色关系需同时查角色文件与 relationships.md）。

## 答题要点

- **信息综合**：角色设定、乐队背景、声优、关系常互相引用，回答要交叉验证。
- **艺名与本名**：RAS 成员用艺名（CHU²/PAREO/LOCK/MASKING/LAYER），档案在本名文件（珠手知由/鳰原令王那/朝日六花/佐藤益木/和奏瑞依），PAREO.md 与 LOCK.md 为软链接。
- **换人史**：声优有更替（如今井莉莎：远藤祐里香→中岛由贵；白金燐子：明坂聪美→志崎桦音；青叶摩卡：三泽纱千香→直田姬奈），回答涉及时注明时期。
- **梗与争议**：查 memes.md / controversies.md，注意梗多源自社区，需给出处与背景。
- **标注来源**：回答重要事实时注明信息出自哪个数据文件（如"出自 data/characters/户山香澄.md"）。
