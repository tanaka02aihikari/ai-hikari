# ai-hikari

会社のマニュアルページ（`index.html`）を複数人で作成・更新するプロジェクトです。

## 公開URL

`main` ブランチに変更がmergeされると、GitHub Actionsが自動でGitHub Pagesに公開します。

https://tanaka02aihikari.github.io/ai-hikari/

## 開発の進め方

1. `main` から作業用ブランチを作成する（例: `add-section-xxx`）
2. `index.html` を編集する
3. ブラウザで直接開いて表示を確認する（ビルド不要）
4. 変更をcommit・pushし、Pull Requestを作成する
5. 他のメンバーのレビューを受けてから `main` にmergeする

mergeされると自動でPages公開に反映されます。

## タスクの管理

追加・修正したい内容はIssueを立てて管理してください。「マニュアルタスク」テンプレートを使うと入力しやすくなります。

## 初回セットアップ（リポジトリ管理者向け）

GitHub Pagesの自動デプロイを有効にするには、リポジトリの Settings → Pages で
Source を **GitHub Actions** に設定してください（初回のみ）。

複数人でのレビューを必須にしたい場合は、Settings → Branches で `main` に対して
「Require a pull request before merging」を設定してください。
