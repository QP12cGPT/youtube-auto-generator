# 🎥 QP動画アップローダー

自動学習AIによってYouTube動画を自動生成・投稿するプロジェクトです。台本から音声・映像・字幕・投稿までを自動化し、将来的にはAI家庭教師のような学習支援も目指しています。

---

## 📦 ディレクトリ構成

project_root/
├── assets/ # 素材フォルダ（音声・背景・キャラ画像など）
│ ├── audio/
│ ├── backgrounds/
│ ├── characters/
│ └── subtitles/
├── output/ # 生成された動画や字幕ファイル
├── scripts/ # 動画生成・アップロード用のPythonスクリプト群
└── README.md # このファイル
---

## ⚙️ 機能一覧

- [x] 台本テキストの読み込み
- [x] CoeFontによる音声自動生成
- [x] 背景画像＋キャラ合成（moviepy）
- [x] 字幕の自動挿入（予定）
- [x] YouTube APIによる自動投稿（審査中）

---

## 🗂 使用方法（例）

```bash
# 台本・音声・画像をassets/に準備した上で
python scripts/generate_video.py
python scripts/upload_to_youtube.py
🔮 今後の開発予定
字幕のタイミング自動生成（pyDub + speech-to-text）

表情・口パク対応（HeyGenなど）

家庭教師型AIとしての拡張

👤 開発者
名前：Naoki Tanaka

AI家庭教師を作る検証としてYouTube自動投稿を実践中

yaml
コピーする
編集する
