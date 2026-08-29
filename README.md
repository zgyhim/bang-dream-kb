# bang-dream-kb

BanG Dream!（邦多利 / 邦邦）企划知识库 Skill。

> **声明**：本项目由 DeepSeek-V4-Flash 生成。

为 AI 助手（opencode）提供邦多利企划的完整离线知识库，数据采集自萌娘百科，按主题分类整理为 Markdown 文件。当用户询问邦多利相关内容时，AI 直接从本知识库检索回答。

## 内容覆盖

- **企划信息**：企划构成、幕后团队、历史沿革、音乐作品、演唱会、媒体活动、衍生作品
- **手游**：《BanG Dream! 少女乐团派对！》游戏简介、登场角色、活动系统、曲目列表
- **9 支乐队**：Poppin'Party、Roselia、Afterglow、Pastel\*Palettes、Hello Happy World!、RAISE A SUILEN、Morfonica、MyGO!!!!!、Ave Mujica
- **45 名角色**：角色设定、性格、经历、人际关系、梗
- **声优信息**：26 位企划相关声优
- **交际网**：队内关系、33 组跨乐队关系、特殊关系
- **企划争议**：13 条争议事件（换人事件、炎上事件、剧情争议等）
- **各种梗**：94 条流行梗（乐队梗 / 角色梗 / 剧情梗 / 社区梗）

## 目录结构

```
bang-dream-kb/
├── SKILL.md                       # Skill 入口（opencode 加载点）
├── README.md                      # 本文件
└── data/
    ├── project_overview.md        # 企划总览
    ├── game_garupa.md             # 手游 少女乐团派对！
    ├── voice_actors.md            # 声优信息
    ├── relationships.md           # 交际网 / 人物关系
    ├── controversies.md           # 企划相关争议
    ├── memes.md                   # 各种梗
    ├── bands/                     # 9 支乐队（每团一文件）
    └── characters/                # 45 名角色（每角色一文件）
```

## 安装 / 使用

本技能作为 opencode 的 skill 使用。opencode 从 skill 目录扫描 `**/SKILL.md` 加载。

```bash
# 方式一：软链接到 opencode 全局 skills 目录
ln -s ~/bang-dream-kb ~/.config/opencode/skills/bang-dream-kb

# 方式二：在 opencode.json 中通过 skills.paths 注册
# "skills": { "paths": ["/home/<user>/bang-dream-kb"] }
```

加载后，询问邦多利相关问题（乐队、角色、声优、关系、梗、争议等）时，AI 会自动查阅 `data/` 下的文件作答。

## 数据说明

- 数据来源：萌娘百科（https://moegirl.icu）
- 角色文件按角色命名；RAS 成员用艺名（CHU²/PAREO/LOCK/MASKING/LAYER），PAREO.md 与 LOCK.md 为本名文件的软链接（鳰原令王那 / 朝日六花）
- 声优有更替历史（如今井莉莎：远藤祐里香 → 中岛由贵；白金燐子：明坂聪美 → 志崎桦音），回答时注意区分时期

## 许可

知识内容整理自萌娘百科，供学习与个人使用。转载或商用请注意原站条款。
