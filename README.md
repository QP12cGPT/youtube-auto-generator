
# 🎥 QP動画アップローダー

自動学習AIによってYouTube動画を自動生成・投稿するプロジェクトです。  
台本から音声・映像・字幕・投稿までを自動化し、将来的には家庭教師のような学習支援AIを目指しています。

---

## 📁 ディレクトリ構成

```
project_root/
├── assets/               # 素材フォルダ（音声・背景・キャラ画像など）
│   ├── audio/
│   ├── backgrounds/
│   ├── characters/
│   └── subtitles/
├── output/               # 生成された動画や字幕ファイル
├── scripts/              # 動画生成・アップロード用のPythonスクリプト群
└── README.md             # このファイル
```

---

## ⚙️ 機能一覧

- ✅ 台本テキストの読み込み
- ✅ CoeFontによる音声自動生成
- ✅ 背景画像＋キャラ合成（moviepy）
- 🔜 字幕の自動挿入（予定）
- 🔜 YouTube APIによる自動投稿（審査中）

---

## 💡 使用方法（例）

```bash
# 台本から音声生成
python scripts/text_to_audio.py --input script.txt

# 動画生成
python scripts/make_video.py

# 字幕追加（予定）
python scripts/add_subtitles.py

# 自動投稿（準備中）
python scripts/upload_youtube.py
```

---

## 📌 今後の進化ステップ

| ステップ         | 内容                                                 |
|------------------|------------------------------------------------------|
| 背景画像・動画合成 | `ImageClip` や `CompositeVideoClip` での合成           |
| 音声自動生成      | `CoeFont API` を使って台本から音声生成                 |
| 字幕タイミング調整 | `pydub` + `speech-to-text` を導入                      |
| YouTube投稿自動化 | `yt-dlp` or `YouTube Data API` を用いた完全自動化        |

---

## 📜 ライセンス

MIT License
