# 3D ビリヤード厚みシミュレーター

Three.js を使った 3D ビリヤード厚みシミュレーターです。手球と的球をドラッグして配置し、角度スライダーで狙いを調整できます。

## 機能

- 3D ビリヤード台（リアルなクッション・ポケット付き）
- 手球・的球のドラッグ配置
- 角度スライダーによる厚み調整
- ゴーストボール表示（当たり位置の可視化）
- サブビュー（手球視点のカメラ）
- OrbitControls によるカメラ操作（回転・ズーム）

## ローカルでの起動方法

ES Modules と importmap を使用しているため、`file://` では動作しません。ローカル HTTP サーバーで起動してください。

```bash
# Python 3
python -m http.server 8000
```

ブラウザで `http://localhost:8000` を開いてください。

## 公開 URL

https://germanium324.github.io/ball-simulator/

## 技術スタック

- [Three.js](https://threejs.org/) v0.160.0 (unpkg CDN / importmap)
- OrbitControls, DragControls (Three.js addons)
- ビルド不要・単一 `index.html` 構成
