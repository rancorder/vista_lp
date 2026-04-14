# VISTA LP

無足場アンカー工法 ランディングページ

## ディレクトリ構成

```
vista-lp/
├── index.html          # メインLP
├── style.css           # スタイルシート
├── main.js             # JS（最小限）
├── vercel.json         # Vercel設定
├── .gitignore
├── public/             # ← Git管理外の大容量ファイル置き場（任意）
├── images/             # 現場写真
│   ├── S__181329927.jpg   （全景・遠景）
│   ├── S__181329929.jpg   （法枠クローズアップ）
│   └── S__181329931.jpg   （施工作業）
└── video/              # PR動画
    └── vista_pr.mp4       ← ここに動画ファイルを配置
```

## デプロイ手順

1. このリポジトリをGitHubにpush
2. [Vercel](https://vercel.com) でリポジトリをインポート
3. Framework Preset: **Other**
4. Root Directory: そのまま（変更不要）
5. Deploy

## 差し替え箇所

| 項目 | ファイル | 場所 |
|------|----------|------|
| 電話番号 | `index.html` | CTAボタンの `href="tel:0X0-XXXX-XXXX"` |
| PR動画 | `video/vista_pr.mp4` | ファイルを置くだけ |

## 注意

- 動画ファイル（`vista_pr.mp4`）はファイルサイズが大きい場合、GitHubの100MB制限に引っかかる可能性があります。
- その場合は **YouTube / Vimeo に限定公開でアップ → `<video>`タグを`<iframe>`に差し替え** を推奨します。
