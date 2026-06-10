# geo-ball

3Dプレビューを見ながら、球状フレームモデルを生成し、STLとしてエクスポートできるシンプルなWebツールです。

## Demo

GitHub Pages:
`https://shinsuke75.github.io/geo-ball/`

## Features

- 球状フレームの3Dプレビュー
- 穴パターンの切り替え
  - 三角 / Triangle
  - 六角 / Hexagon
- ビーム断面形状の切り替え
  - 三角 / Triangle
  - 四角 / Square
  - 円 / Circle
- パラメータ調整
  - 直径 / Diameter
  - 枠の太さ / Frame Thickness
  - 形状分割レベル / Mesh Division Level
- STLエクスポート
- タッチ操作対応

## Usage

### Parameters

- **穴の形状 / Hole Pattern**
  - 三角 / Triangle
  - 六角 / Hexagon

- **断面形状 / Beam Shape**
  - 三角 / Triangle
  - 四角 / Square
  - 円 / Circle

- **直径 / Diameter (mm)**
  - モデル全体の直径

- **枠の太さ / Frame Thickness (mm)**
  - フレームの太さ

- **形状分割レベル / Mesh Division Level (0–5)**
  - 値を大きくすると形状が細かくなる代わりに、処理が重くなります

### Controls

#### Desktop
- 左ドラッグ: 回転
- 右ドラッグ: パン
- マウスホイール: ズーム

#### Touch devices
- 1本指ドラッグ: 回転
- 2本指操作: パン / ピンチズーム

### Export

- `STLを生成 / Export STL` ボタンで STL ファイルを保存できます

## Notes

- 分割レベルを高くすると、プレビュー更新やエクスポートに時間がかかる場合があります
- ブラウザや端末性能によって動作速度が変わります
- STLはモデリング用途を想定した出力です。造形前にスライサー等で最終確認してください

## Tech

- HTML
- JavaScript
- Three.js

## Development

現在は単一の `index.html` に UI / geometry / viewer / export が含まれています。  
今後の改善候補:

- README拡充
- Reset View ボタン追加
- フォームのアクセシビリティ改善
- JavaScript の分割整理
- 重い処理時のUX改善

## License

ライセンス未設定
