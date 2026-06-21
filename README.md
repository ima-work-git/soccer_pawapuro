# soccer_pawapuro

日本代表 vs チュニジア（キリンカップ2022）のスタメン11人を、
パワプロ風の能力値カードで表示するWebページです。

## 画面

- `index.html` … 単一ファイルのフロントエンド（HTML/CSS/JSのみ、ビルド不要）
  - スタメン11人をパワプロ風カードで表示（総合ランク・各能力のS〜Gランク＋カラーバー・特殊能力チップ）
  - ポジション（GK / DF / MF / FW）で絞り込み可能

> 能力値・特殊能力はパワプロ風に演出したファンメイドの査定で、公式データではありません。

## デプロイ（GitHub Pages）

`.github/workflows/deploy.yml` が、`claude/japan-tunisia-player-stats-bdkh2k` /
`main` への push 時に `index.html` を **`gh-pages` ブランチ** へ公開します。

### 初回のみ：Pages の有効化が必要

このリポジトリではまだ GitHub Pages が有効化されていないため、
公開コンテンツ（`gh-pages` ブランチ）は準備済みですが配信されていません。
オーナーが一度だけ以下を設定してください。

1. リポジトリの **Settings → Pages** を開く
2. **Build and deployment → Source** を **「Deploy from a branch」** に
3. **Branch** を **`gh-pages`** / **`/ (root)`** にして **Save**

数十秒〜数分後、次のURLで公開されます：

**https://ima-work-git.github.io/soccer_pawapuro/**

以降は対象ブランチへ push するたびに自動で更新されます。
