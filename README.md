# seedance-refs

「李白漫游系列」的公开参考素材库。Seedance / MiniMax H3 只能抓公网 https 直链，所以素材放在这里，用 raw 直链引用。

引用规则：一律用 `https://raw.githubusercontent.com/kaka20211019/seedance-refs/main/<路径>`，不要用 GitHub 页面（blob）链接。

## 角色设定 / 故事版参考

- `assets/series_foundation_contact_sheet.png` — 系列基础角色设定参考图（故事版用）
  https://raw.githubusercontent.com/kaka20211019/seedance-refs/main/assets/series_foundation_contact_sheet.png

## 声音参考

**李白的声音基准（系列统一使用）**
- `assets/voice/libai_voice_early_baidi_city_4lines.wav` — 10.8 秒，44.1kHz 单声道 WAV
  https://raw.githubusercontent.com/kaka20211019/seedance-refs/main/assets/voice/libai_voice_early_baidi_city_4lines.wav
  来源：《早发白帝城》成片（MiniMax H3 原生混音）经 Demucs 人声分离，按四句诗切出后合并，句间 0.5 秒静音。
  第四句底下有轻微猿叫叠音（原片设定），其余三句干净。
  用法：MiniMax H3 `reference_audios` 填此直链，提示词写"用参考音频 1 的声音"，并把台词放在引号里。

放新样本的规则：WAV/MP3，每段 2–15 秒、合计 ≤15 秒，单人干净人声。

## 上传方式

本机 `D:\Seedance-MCP` 里：`node scripts/publish-ref.mjs <本地文件> --dir assets`（音频可用 `--dir assets/voice`）。
MCP 的 `reference_audios` 给本地 wav/mp3 路径时会自动走这一步（环境变量 `SEEDANCE_REFS_REPO=kaka20211019/seedance-refs`）。
