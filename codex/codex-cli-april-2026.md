## Windows サンドボックスのネットワーク制御強化

Windows サンドボックスにおいて、環境変数に頼らず OS レベルの egress（外向き通信）ルールによるプロキシ限定ネットワーク接続の強制が可能になった。より厳密な隔離環境の構築が実現する。

[参考リンク](https://developers.openai.com/codex/changelog)

## ChatGPT サインインのデバイスコードフロー対応

アプリサーバークライアントが ChatGPT サインインをデバイスコードフローで開始できるようになった。ブラウザコールバックによるログインが不安定・利用不可な環境でも認証できる。

[参考リンク](https://developers.openai.com/codex/changelog)

## codex exec のプロンプト＋標準入力ワークフロー対応

`codex exec` でプロンプトと標準入力を同時に扱えるようになり、パイプで入力を渡しつつコマンドライン引数で別途プロンプトを指定するワークフローに対応した。

[参考リンク](https://developers.openai.com/codex/changelog)

## カスタムモデルプロバイダーの動的トークンリフレッシュ

カスタムモデルプロバイダーで、短命な bearer トークンを動的に取得・リフレッシュできるようになった。設定ファイルや環境変数の静的認証情報に縛られずに済む。

[参考リンク](https://developers.openai.com/codex/changelog)

## リモート／アプリサーバーワークフローの拡充

egress 通信用の WebSocket トランスポート、remote `--cd` 転送、ランタイムでのリモート制御有効化、サンドボックス対応のファイルシステム API、実験的サブコマンド `codex exec-server` が追加され、リモート開発ワークフローが大幅に強化された。

[参考リンク](https://developers.openai.com/codex/changelog)

## TUI の利便性向上

TUI で最新のエージェント応答を `Ctrl+O` でコピー可能に。`/resume` からセッション ID または名前で直接ジャンプできるようになり、TUI 通知の設定項目も増えた。また、レートリミット取得を非同期化し、TUI の起動が高速化された。

[参考リンク](https://developers.openai.com/codex/changelog)

## GPT-5.3-Codex-Spark のリサーチプレビュー公開

GPT-5.3-Codex の小型版にあたる「GPT-5.3-Codex-Spark」のリサーチプレビューが公開された。リアルタイムコーディング向けに設計された初のモデルで、毎秒 1000 トークンを超える応答速度を実現しつつ、実用的なコーディングタスクに必要な能力を維持する。テキストのみ対応、128k のコンテキストウィンドウを備える。

[参考リンク](https://openai.com/index/introducing-gpt-5-2-codex/)

## ChatGPT サインイン時の利用可能モデルの整理（2026年4月14日）

Codex for ChatGPT にサインインした際に選択できるモデルが整理され、古いモデルが削除された。現在利用可能なのは `gpt-5.4`、`gpt-5.4-mini`、`gpt-5.3-codex`、`gpt-5.2`。ChatGPT Pro ユーザーは `gpt-5.3-codex-spark` も選択できる。

[参考リンク](https://developers.openai.com/codex/changelog)
