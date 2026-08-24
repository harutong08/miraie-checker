# ミライエ（制震壁）配置判定ツール

図面画像を貼ると自動でOCR読み取りし、制震壁の配置基準
`|(M1+…+Mn) − (G×n)| ≦ L/3` を判定するツールです。

- `index.html`：HTML/CSS/JSを内包した単一ファイル。画像OCR（Tesseract.js）はCDNから読み込みます。
- `manifest.json`：アプリ名・アイコン・単独ウィンドウ表示の設定
- `sw.js`：サービスワーカー。オンライン時は常に最新を取得し、オフライン時のみキャッシュにフォールバック
- `icons/`：アプリアイコン（192px・512px）
- ホスティング：GitHub Pages（`main`ブランチのルートを配信）

## 更新のしかた

1. `index.html` を編集する
2. コミットして `main` ブランチへ push する
3. 数十秒〜1分ほどでGitHub Pagesに自動反映される（`manifest.json` や `icons/` を変えたときも同様）

開発元リポジトリ（検証キット・仕様メモ含む）: [harutong08/-](https://github.com/harutong08/-)
