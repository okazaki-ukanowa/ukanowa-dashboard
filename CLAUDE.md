# うかのわ Claude Code 起動ルール

## 起動時に必ず実行すること

作業開始前に必ず以下を実行し、next_action / status / blocker を読んで現在地を把握する。

curl -s "https://ukanowa-api.commonground-oka.workers.dev/context?pj=%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E9%96%8B%E7%99%BA"

説明なしで即作業開始できる状態になってから手を動かすこと。

## コード変更ルール

- コードは完全書き換えのみ。部分編集しない
- 変更後は必ずGitHubにプッシュする（ローカルで終わらせない）
- Cloudflare Worker URL は変更禁止：https://ukanowa-api.commonground-oka.workers.dev
- Notion APIキーはコードに書かない（Worker環境変数 NOTION_TOKEN 経由）

## 参照先

- 引き継ぎ資料：https://www.notion.so/32a43c0d960c817cb9b4ef79c842fe6c
