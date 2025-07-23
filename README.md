# WSI Viewer

病理画像WSI（Whole Slide Image）ビューアーアプリケーション

## 概要

このプロジェクトは、ブラウザ上で病理画像のWSI形式ファイルを表示・閲覧するためのWebアプリケーションです。

## 特徴

- ブラウザベースでの高解像度WSI画像表示
- ズーム・パン操作によるスムーズな閲覧
- 複数のWSI形式に対応
- レスポンシブデザイン

## 対応形式

- Deep Zoom Image (.dzi)
- Zoomify
- IIIF (International Image Interoperability Framework)
- OpenSlide対応形式 (SVS, NDPI, TIFFなど)

## ディレクトリ構造

```
wsi-viewer/
├── index.html                 # メインページ
├── css/
│   ├── style.css             # メインスタイル
│   └── viewer.css            # ビューアー専用スタイル
├── js/
│   ├── app.js                # メインアプリケーション
│   ├── viewer.js             # ビューアー制御
│   └── utils.js              # ユーティリティ関数
├── lib/
│   └── openseadragon/        # OpenSeadragonライブラリ
├── assets/
│   ├── images/               # UI用画像
│   └── icons/                # アイコン類
├── samples/
│   ├── sample.dzi            # サンプルDZI
│   └── sample_files/         # サンプル画像タイル
├── docs/
│   ├── README.md             # プロジェクト説明
│   └── usage.md              # 使用方法
└── server/
    └── simple-server.py      # Python簡易サーバー
```

## セットアップ

1. リポジトリをクローン
2. 簡易サーバーを起動（CORS対応のため）
3. ブラウザでアクセス

## 使用技術

- OpenSeadragon.js - 高解像度画像表示ライブラリ
- HTML5/CSS3/JavaScript
- Python（開発用サーバー）

## ライセンス

MIT License