# seedance-refs

「李白漫游系列」的公开参考素材库。Seedance / MiniMax H3 只能抓公网 https 直链，所以素材放在这里，用 raw 直链引用。

引用规则：一律用 `https://raw.githubusercontent.com/kaka20211019/seedance-refs/main/<路径>`，不要用 GitHub 页面（blob）链接。

## 角色设定 / 故事版参考

- `assets/series_foundation_contact_sheet.png` — 系列基础角色设定参考图（故事版用）
  https://raw.githubusercontent.com/kaka20211019/seedance-refs/main/assets/series_foundation_contact_sheet.png

## 声音参考（待补）

`assets/voice/` 下放角色声音基准样本（WAV/MP3，每段 2–15 秒，干净无背景音），供 MiniMax H3 `reference_audios` 使用。

## 上传方式

本机 `D:\Seedance-MCP` 里：`node scripts/publish-ref.mjs <本地文件> --dir assets`（音频可用 `--dir assets/voice`）。
MCP 的 `reference_audios` 给本地 wav/mp3 路径时会自动走这一步（环境变量 `SEEDANCE_REFS_REPO=kaka20211019/seedance-refs`）。
