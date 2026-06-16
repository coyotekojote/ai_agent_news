## ブロックされた画像添付のガイダンス改善

ブロックされた画像添付に対して、「Editor preview features」ポリシーでのビジョン有効化、ビジョン対応モデルへの切り替え、別の画像の試行などの具体的なガイダンスが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## --helpオプションのアルファベット順ソート

`--help` 出力のオプションがアルファベット順にソートされるようになった。デュアルロングフラグを持つオプションも含まれる。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## 認証エラーの可視性向上

サインインバナーに認証バリデーション失敗とネットワークアクセスガイダンスが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## フォークベースPRの表示

フォークベースのプルリクエストが `/pr` コマンドとブランチPRバッジに表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## リモートセッションのケース非依存リジューム

ローカルとリモートのリポジトリ名が大文字小文字のみ異なる場合でもセッションをリジュームできるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## スピルファイルパスの表示

read_bash出力がサイズ制限を超えた場合にスピルファイルのパスが表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## /chronicleスタンダップのローカルセッション追加

`/chronicle` スタンダップに最近のローカルセッションが含まれるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## WebSocket接続の復元

`/responses` WebSocket接続が復元された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## 一時的な401エラーのリトライ

HMACおよびOAuthモードでの一時的な401エラーが自動的にリトライされるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## diffでの空白変更非表示

`/diff` で `w` キーを押すと空白のみの変更が非表示になるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## MCP deferToolsオプションの追加

MCPサーバー設定に `deferTools` オプションが追加され、ツール検索中もサーバーツールの利用可能性が維持されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## エージェントモードのセッション単位追跡

エージェントモードがセッション単位で追跡されるようになり、セッション間で永続化されなくなった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## Windowsクラッシュの防止

ホストプロセスのヒープが破損した場合のネイティブランタイムアドオンクラッシュが防止された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## ネイティブドキュメント添付の復旧

読み取り不能なネイティブドキュメント添付がファイルパスアップロードにフォールバックするようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## PostToolUseフックマッチャーの修正

フックマッチャー（例: `Edit|Write`）が正しく適用されるようになり、フォーマッターやリンターが対象ツールの後にのみ実行されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## APIリクエストの信頼性向上

OpenAI、Anthropic、Azure OpenAIへのリクエストの信頼性が向上した。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## 実験的/rewindコマンドの改善

`/rewind` がgit非依存になり、ユーザーの編集を保持しつつCopilotの変更のみを選択的に復元できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## 逆検索入力フッターの整列修正

コマンド履歴ブラウジング中の逆検索入力フッターの整列が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## Issue詳細のEnterキーナビゲーション

ハイライトされたIssueでEnterキーを押すと詳細が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)

## OpenAI互換バックエンドでのプランレビュー修正

厳密なOpenAI互換バックエンドでプランレビューメニューが正しく機能するようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.63)
