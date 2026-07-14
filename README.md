# Elegant Penguin Orchestra

一群高雅人士企鹅组成的 Codex 像素乐团。

每位企鹅演奏一种不同的乐器，每种乐器都是一个可以独立安装和选择的 Codex pet。乐团成员会逐个补充；目前完成的第一位成员是萨克斯企鹅。

## 当前成员

| 成员 | 乐器 | Pet ID | 状态 |
| --- | --- | --- | --- |
| Saxphone Penguin | 萨克斯 | `saxphone` | 已完成 |

## 安装萨克斯企鹅

将 [`saxphone`](saxphone) 文件夹复制到：

```text
%USERPROFILE%\.codex\pets\saxphone
```

然后在 Codex 中打开 **Settings > Pets**，刷新宠物列表并选择 **Saxphone Penguin**。在任务中输入 `/pet` 即可唤出。

它是 Codex Desktop 自定义宠物，不是独立的 Windows 桌宠，不需要 Python 或其他运行依赖。

## 项目结构

每种乐器使用一个独立目录，运行时目录中只需要 `pet.json` 和 `spritesheet.webp`：

```text
elegant-penguin-orchestra/
├── saxphone/                 # 第一位成员：萨克斯企鹅
│   ├── pet.json
│   └── spritesheet.webp
└── xiaohongshu/              # 宣传动图，不参与宠物运行
```

以后新增乐器时，会继续以相同结构添加新的 pet 目录。

## Codex 宠物图集规格

- 图集：1536 × 1872、8 列 × 9 行、透明 WebP
- 单帧：192 × 208
- 动作：idle、running-right、running-left、waving、jumping、failed、waiting、running、review