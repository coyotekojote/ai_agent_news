## /cd によるワーキングディレクトリの永続化

`/cd` でワーキングディレクトリが永続化されるようになり、セッション再開時にそのディレクトリに戻り、新しいディレクトリのカスタムエージェントが検出されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## スラッシュプレフィックス引数の誤検知修正

`--body "/azp run"` などスラッシュプレフィックスの文字列引数がファイルシステムのパーミッションプロンプトを誤ってトリガーしなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## フルスクリーンタイムラインのアンカリング

古いコンテンツがトリミングされた際にフルスクリーンタイムラインがアンカーを維持するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## キャンバスの自動再開

CLI 再起動後にオープンしていたキャンバスが自動的に再開されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## CI ステータスバー表示

現在のブランチの CI チェックステータス（passing/running/failing）を表示するオプションのステータスバー項目が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## copilot skill サブコマンドの追加

`copilot skill` サブコマンドおよび `/skill` エイリアスが追加され、ファイル、URL、ディレクトリからスキルの一覧表示・追加・削除が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## GitHub テーマ起動時フラッシュの修正

非 GitHub テーマ使用時に起動時に GitHub 背景が一瞬表示される問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## Windows コンソールウィンドウのフラッシュ修正

エージェントがフックコマンドを実行する際に Windows のコンソールウィンドウが一瞬表示される問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## userPromptSubmitted フックの additionalContext 対応

`userPromptSubmitted` フックの `additionalContext` がモデル向けプロンプトに含まれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## Windows パスの保持

stdio MCP サーバー追加時に Windows パスが保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## MCP シャットダウンの改善

MCP シャットダウンがインフライトのサーバー接続を待たなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## CLI 再起動の最適化

シャットダウンタイムアウトなしで CLI が再起動されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## タイムラインのシェルコマンドシンタックスハイライト削除

タイムラインでのシェルコマンドのシンタックスハイライトが削除された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## カスタムエージェントモデル選択の永続化

BYOK プロバイダー使用時にカスタムエージェントのサブエージェントモデル選択が保持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## /every スケジュールのパース改善

`/every` スケジュールがセッションのメインモデルでパースされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## tmux でのインライン画像レンダリング修正

tmux でインライン画像が確実にレンダリングされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## ask_user フリーフォームのテキスト折り返し改善

`ask_user` のフリーフォームオプションでテキストが折り返され、カーソルが整列されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## カスタムステータスラインコマンドの設定保存

カスタムステータスラインコマンドが `/settings` に保存されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## ストリーミングバイトカウントの分離表示

ストリーミングバイトカウントがキャンセルヒントとは別に表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## セルフペースドスケジュール非アクティブ時のウェイクアップ処理

セルフペースドスケジュールがアクティブでない場合のウェイクアップミスファイアが適切に処理されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## MCP OAuth リフレッシュの改善

サイレント MCP OAuth リフレッシュが付与済みスコープを再利用し、永続的なサインインが維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)

## シェルコマンド履歴の拡張

通常モードで上下キー履歴と Ctrl+R の逆方向検索に過去のシェルコマンドが含まれるようになり、シェルモードに入らずにコマンドの呼び出しと再実行が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.65)
