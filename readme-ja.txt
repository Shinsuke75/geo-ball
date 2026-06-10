geo-ball v11.6.0（Triangle & Hexagon）
=====================================
- 四角（Square）は別アプリに分離済み。本アプリは三角・六角のみ。
- どちらも面接地になるように向きを自動調整 → 出力前にz=0フロアリング＋微小負値クランプ。
- 退化三角形は除去してクリーンなSTLを生成。

デプロイ方法（Netlify）
-----------------------
1. このZIPを解凍して、`index.html` を Netlify の Drag & Drop に渡すか、
   リポジトリに `index.html` を追加してデプロイしてください。
2. Node バージョン固定が必要なら、プロジェクト側で `package.json` の engines.node か
   `netlify.toml` の NODE_VERSION を設定してください。

更新日時: 2025-10-15T14:00:39