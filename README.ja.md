# kofun

ブラウザ上で日本の古墳の3Dモデルをレンダリングするサンプルのコレクションです。このプロジェクトでは、Three.jsとA-Frameを使用してVRML 1.0モデルを読み込み、表示するためのさまざまな方法を紹介しています。

## デモ

- **[ソリッドモデルビューアー (Three.js)](https://code4fukui.github.io/kofun/kofun.html)**: 標準のThree.js `VRMLLoader`を使用してソリッドモデルをレンダリングする、オービットコントロールを備えたインタラクティブなビューアー。
- **[ワイヤーフレームビューアー (Three.js)](https://code4fukui.github.io/kofun/test.html)**: JavaScriptで独自に実装したVRMLパーサーを使用したワイヤーフレームの可視化。
- **[基本的なシーン (A-Frame)](https://code4fukui.github.io/kofun/aframe.html)**: カスタムコンポーネントを使用してA-Frameのシーン内にVRMLモデルを読み込むシンプルなデモ。

## 特徴

- **複数のレンダリングアプローチ**: 以下の方法でVRML 1.0モデルをレンダリングするデモを提供します:
  - 標準のThree.js `VRMLLoader` (`kofun.html`)
  - スクラッチから作成した独自のVRMLパーサー (`test.html`)
  - A-Frameのカスタムコンポーネント (`aframe.html`)
- **インタラクティブなビューアー**: Three.jsの2つのサンプルには、モデルを観察するためのインタラクティブなオービットコントロールが組み込まれています。
- **VRMLデータ**: 古墳の多層的なジオメトリを表現する `.wrl` (VRML 1.0) ファイルを使用しています。

## 使い方

ブラウザのセキュリティポリシーにより、ファイルシステムから直接モデルを読み込むことは制限されているため、これらのサンプルをローカルで実行するには、ローカルWebサーバーからファイルを提供する必要があります。

1. リポジトリをクローンします:
    ```sh
    git clone https://github.com/code4fukui/kofun.git
    ```
2. プロジェクトのディレクトリに移動します:
    ```sh
    cd kofun
    ```
3. シンプルなローカルWebサーバーを起動します（例: Pythonを使用）:
    ```sh
    # Python 3の場合
    python -m http.server
    ```
4. ブラウザで以下のいずれかのサンプルファイルを開きます:
    - `http://localhost:8000/kofun.html`
    - `http://localhost:8000/test.html`
    - `http://localhost:8000/aframe.html`

## データソース

古墳のVRMLモデルは、堺市が提供するデータに基づいています。

- [三大古墳の3D比較](https://www.city.sakai.lg.jp/kanko/rekishi/dkofun/3dhikaku/funbohikaku.html)

## ライセンス

MIT License — 詳細は [LICENSE](LICENSE) を参照してください。
