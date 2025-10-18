# ikeisuke.github.io

このリポジトリは、ikeisuke の GitHub Pages（ユーザーサイト）として、各アプリのポリシーや簡易ドキュメントをまとめて公開するためのベースです。

## 全体方針

- 目的: 各アプリのプライバシーポリシー等を安定URLで一元公開
- 構成: Jekyll + 最小レイアウト、データ駆動でアプリ一覧を生成
- 情報設計: `apps/<app>/privacy/` にアプリ別ポリシーを配置、トップから一覧導線
- コンテンツ: 日本語を基準に簡潔・明確に。実装確定後に具体項目を追記
- 運用: 既存別レポジトリの移管は別Issue/PRで段階的に対応（本リポジトリではTumbliumのみ先行）

## 構成

- `_config.yml` — サイト設定
- `_layouts/default.html` — 共通レイアウト
- `_data/apps.yml` — アプリ一覧データ
- `index.md` — トップページ（アプリ一覧を表示）
- `apps/<app>/privacy/index.md` — 各アプリのプライバシーポリシー

## 追加方法（新しいアプリのポリシー）

1. ページを追加:
   - 例: `apps/myapp/privacy/index.md`
   - 先頭に以下のFront Matterを設定:
     ```
     ---
     layout: default
     title: MyApp プライバシーポリシー
     ---
     ```
   - 本文にポリシー本文を記載（`apps/tumblium/privacy/index.md` を雛形として利用可能）

2. アプリ一覧に登録:
   - `_data/apps.yml` に以下を追加:
     ```yaml
     - id: myapp
       name: MyApp
       links:
         privacy: /apps/myapp/privacy/
     ```

3. お問い合わせの案内（推奨）:
   - 原則、メールアドレスは記載せず「アプリ内のヘルプ／サポートから連絡」を案内します。
   - どうしてもメール掲載が必要な場合のみ、合意の上で `_config.yml` の `contact.email` を利用。

## 運用メモ

- GitHub Pages のユーザーサイト（`ikeisuke.github.io`）としてビルドされます。
- テーマ依存を最小化するため、素朴なレイアウトで構成しています。
- 既存レポジトリで運用しているドキュメント（例: MimiLoopDocs）を段階的にこちらへ移管可能です。

## 本対応の範囲

- 本コミットでは「Tumblium」のプライバシーポリシーのみを公開対象としています。
- 他アプリ（例: MimiLoop）の移管は別途Issue/PRで対応します。
