# Elegant Penguin Orchestra

一群高雅人士企鹅组成的 Codex 像素乐团。

每位企鹅演奏一种不同的乐器，每种乐器都是一个可以独立安装和选择的 Codex pet。乐团成员会逐个补充，目前已有 17 位成员，涵盖西洋管弦乐器、电声乐器、打击乐器与中国民族乐器。

## 当前成员

| 成员 | 乐器 | Pet ID | 状态 |
| --- | --- | --- | --- |
| Saxphone Penguin | 萨克斯 | `saxphone` | 已完成 |
| Suona Penguin | 唢呐 | `suona` | 已完成 |
| Trombone Penguin | 长号 | `trombone` | 已完成 |
| Flute Penguin | 长笛 | `flute` | 已完成 |
| French Horn Penguin | 圆号 | `french-horn` | 已完成 |
| Clarinet Penguin | 单簧管 | `clarinet` | 已完成 |
| Bass Penguin | 贝斯 | `bass` | 已完成 |
| Cello Penguin | 大提琴 | `cello` | 已完成 |
| Tuba Penguin | 大号 | `tuba` | 已完成 |
| Liuqin Penguin | 柳琴 | `liuqin` | 已完成 |
| Piano Penguin | 钢琴 | `piano` | 已完成 |
| Guzheng Penguin | 古筝 | `guzheng` | 已完成 |
| Trumpet Penguin | 小号 | `trumpet` | 已完成 |
| Drum Kit Penguin | 架子鼓 | `drum-kit` | 已完成 |
| Oboe Penguin | 双簧管 | `oboe` | 已完成 |
| Bassoon Penguin | 巴松 | `bassoon` | 已完成 |
| Guitar Penguin | 吉他 | `guitar` | 已完成 |

## 安装宠物

将想使用的宠物目录复制到 `%USERPROFILE%\.codex\pets` 下。例如：

```text
%USERPROFILE%\.codex\pets\saxphone
%USERPROFILE%\.codex\pets\suona
%USERPROFILE%\.codex\pets\trombone
%USERPROFILE%\.codex\pets\flute
%USERPROFILE%\.codex\pets\french-horn
%USERPROFILE%\.codex\pets\clarinet
%USERPROFILE%\.codex\pets\bass
%USERPROFILE%\.codex\pets\cello
%USERPROFILE%\.codex\pets\tuba
%USERPROFILE%\.codex\pets\liuqin
%USERPROFILE%\.codex\pets\piano
%USERPROFILE%\.codex\pets\guzheng
%USERPROFILE%\.codex\pets\trumpet
%USERPROFILE%\.codex\pets\drum-kit
%USERPROFILE%\.codex\pets\oboe
%USERPROFILE%\.codex\pets\bassoon
%USERPROFILE%\.codex\pets\guitar
```

然后在 Codex 中打开 **Settings > Pets**，刷新宠物列表并选择想使用的乐团成员。在任务中输入 `/pet` 即可唤出。

它是 Codex Desktop 自定义宠物，不是独立的 Windows 桌宠，不需要 Python 或其他运行依赖。

## 项目结构

每种乐器使用一个独立目录，运行时目录中只需要 `pet.json` 和 `spritesheet.webp`：

```text
elegant-penguin-orchestra/
├── saxphone/                 # 萨克斯企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── suona/                    # 唢呐企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── trombone/                 # 长号企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── flute/                    # 长笛企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── french-horn/              # 圆号企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── clarinet/                 # 单簧管企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── bass/                     # 贝斯企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── cello/                    # 大提琴企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── tuba/                     # 大号企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── liuqin/                   # 柳琴企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── piano/                    # 钢琴企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── guzheng/                  # 古筝企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── trumpet/                  # 小号企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── drum-kit/                 # 架子鼓企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── oboe/                     # 双簧管企鹅
│   ├── pet.json
│   └── spritesheet.webp
├── bassoon/                  # 巴松企鹅
│   ├── pet.json
│   └── spritesheet.webp
└── guitar/                   # 吉他企鹅
    ├── pet.json
    └── spritesheet.webp
```

以后新增乐器时，会继续以相同结构添加新的 pet 目录。

## Codex 宠物图集规格

- 图集：1536 × 1872、8 列 × 9 行、透明 WebP
- 单帧：192 × 208
- 动作：idle、running-right、running-left、waving、jumping、failed、waiting、running、review
