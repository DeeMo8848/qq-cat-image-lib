# 🖼️ QQ 猫猫机器人图库

供给 **qq-cat-bot** 使用的本地图片类素材资源仓库。

⚠️ 私有仓库。安装脚本拉取本仓库需提供只读访问令牌（GitHub PAT）。

## 目录结构

```
dragon/    ← 本地「随机龙」使用的龙图素材（随机图像模块「随机龙」从这里取图）
```

目前仅含 `dragon/` 一个子目录；后续可继续添加其他图类素材子目录（作为次级目录存放）。

## 使用（在 qq-cat-bot 项目内）

```powershell
# 拉取图库到项目 resources/image_lib，DRAGON_DIR 会自动解析到其 dragon/ 子目录
powershell -ExecutionPolicy Bypass -File .\install.ps1
```

bot 启动后，`config.py` 会自动把 `DRAGON_DIR` 默认指向 `resources/image_lib/dragon`，
无需在 `settings.json` 里手动填写。也可在 `settings.json` 的 `DRAGON_DIR` 里显式覆盖。

## 更新素材

新增/替换龙图后推送到本仓库，重新运行 install.ps1 或在 bot 里重新拉取即可同步。

## 说明

素材为个人收藏整理，仅用于自用机器人，请勿用于公开商业用途。