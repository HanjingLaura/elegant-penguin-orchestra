# Elegant Penguin Orchestra

![Elegant Penguin Orchestra](social/readme-banner.png)

[简体中文](README.md) | [English](README_EN.md)

## About

**Elegant Penguin Orchestra** is a pixel-art custom pet collection for **Codex Desktop**. Its 23 matching penguin performers wear fedoras, square sunglasses, and ties while each playing a different instrument. Every member is packaged as an independently installable pet.

Phase one is complete. This 23-member edition is the project's current stopping point. Any future additions will follow the same character design, animation specification, and directory convention.

> These are custom pets for Codex Desktop. They are not standalone Windows desktop pets and do not include a separately runnable executable.

## Orchestra Members

| # | Member | Instrument | Pet ID |
| ---: | --- | --- | --- |
| 1 | Saxophone Penguin | Saxophone | `saxphone` |
| 2 | Suona Penguin | Suona | `suona` |
| 3 | Trombone Penguin | Trombone | `trombone` |
| 4 | Flute Penguin | Flute | `flute` |
| 5 | Violin Penguin | Violin | `violin` |
| 6 | French Horn Penguin | French horn | `french-horn` |
| 7 | Clarinet Penguin | Clarinet | `clarinet` |
| 8 | Bass Penguin | Electric bass | `bass` |
| 9 | Cello Penguin | Cello | `cello` |
| 10 | Tuba Penguin | Tuba | `tuba` |
| 11 | Baritone Horn Penguin | Baritone horn | `baritone-horn` |
| 12 | Liuqin Penguin | Liuqin | `liuqin` |
| 13 | Piano Penguin | Piano | `piano` |
| 14 | Guzheng Penguin | Guzheng | `guzheng` |
| 15 | Erhu Penguin | Erhu | `erhu` |
| 16 | Trumpet Penguin | Trumpet | `trumpet` |
| 17 | Drum Kit Penguin | Drum kit | `drum-kit` |
| 18 | Cymbals Penguin | Crash cymbals | `cymbals` |
| 19 | Marimba Penguin | Marimba | `marimba` |
| 20 | Maracas Penguin | Maracas | `maracas` |
| 21 | Oboe Penguin | Oboe | `oboe` |
| 22 | Bassoon Penguin | Bassoon | `bassoon` |
| 23 | Guitar Penguin | Guitar | `guitar` |

> The legacy Pet ID `saxphone` is retained for compatibility with existing installations; the instrument and display name use the correct spelling, Saxophone.

## Installation

1. Choose a pet directory from the repository, such as `tuba/`.
2. Copy the entire directory to:

   ```text
   %USERPROFILE%\.codex\pets\<pet-id>
   ```

   For example, install the tuba pet at:

   ```text
   %USERPROFILE%\.codex\pets\tuba
   ```

3. Open **Settings > Pets** in Codex Desktop and select the installed member.
4. Restart Codex Desktop if the pet list does not refresh.
5. Enter `/pet` in a Codex task to summon the selected pet.

Only the selected pet directory is required for installation. The `social/` directory is not part of the runtime package.

## Pet Package Structure

Each instrument has its own directory. A runnable pet package contains only two files:

```text
<pet-id>/
├── pet.json
└── spritesheet.webp
```

- The directory name must match the `id` in `pet.json`.
- `pet.json` stores the display name, description, and spritesheet path.
- `spritesheet.webp` is the transparent animation atlas loaded by Codex Desktop.
- `social/` contains the README banner and Xiaohongshu portrait cover; it is not used at runtime.

## Animation Atlas Specification

| Item | Specification |
| --- | --- |
| File | `spritesheet.webp` |
| Canvas | 1536 × 1872 |
| Format | WebP with transparency |
| Grid | 8 columns × 9 rows |
| Frame | 192 × 208 |
| Populated frames | 57 |

Animation rows are fixed in this top-to-bottom order:

| Row | Action | Frames |
| ---: | --- | ---: |
| 1 | `idle` | 6 |
| 2 | `running-right` | 8 |
| 3 | `running-left` | 8 |
| 4 | `waving` | 4 |
| 5 | `jumping` | 5 |
| 6 | `failed` | 8 |
| 7 | `waiting` | 6 |
| 8 | `running` | 6 |
| 9 | `review` | 6 |

Unused cells and the atlas background remain transparent.
