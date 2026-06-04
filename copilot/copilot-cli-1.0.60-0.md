## 課金ヘルプトピックの追加

AIクレジット使用機能に関する課金ヘルプトピックが追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.60-0)

## /diffビューのVimスタイルナビゲーション

/diffビューでVimスタイルのナビゲーションキー（g、G、Ctrl+D、Ctrl+U）が使用可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.60-0)

## Mission Control共有ステータスの表示

/session infoビューにMission Controlの共有ステータスが表示されるようになった。セッションリンクの表示も改善された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.60-0)

## --resumeの短縮フラグ

`--resume`フラグの短縮形として`-r`が追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.60-0)

## LSPサーバー設定の強化

LSPサーバー設定でbash、powershell、cwdキーがサポートされ、プラグイン変数展開が可能になった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.60-0)

## PRからのgit worktree作成

プルリクエスト画面から直接git worktreeを作成できるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.60-0)

## Rewindピッカーの改善

Rewindピッカーの各チェックポイントにワーキングツリーのdiff統計（+追加 -削除）が表示されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.60-0)

## その他の改善

/envコマンドでフック数とソース出所が表示されるようになった。

/helpコンテンツにキーボードショートカットが追加された。

ベアな#number形式のissue/PR参照が現在のリポジトリに自動リンクされるようになった。

--cloudの実験モード要件に関するエラーメッセージが改善された。

/tasksの詳細ビューでフォローアップメッセージ後に最新のプロンプトが表示されるようになった。

`--allow-all-tools`、`--allow-all-paths`、`--allow-all-urls`のバイパス権限が強制されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.60-0)

## バグ修正

制限超過ユーザーの負のパーセンテージ表示が修正された。

拡張機能の権限プロンプトが`--yolo`および事前承認された場所を尊重するようになった。

カスタムエージェント指示がターンをまたいで重複する問題が修正された。

LinuxサンドボックスのallowedHosts/blockedHosts設定との互換性が修正された。

セッション完了シグナルがバックグラウンドシェルコマンドを適切に待機するようになった。

macOSでのCmd+Backspaceによる行削除が修正された。

`web_fetch`がループバック、プライベート、メタデータアドレスをブロックするようになった。

並行実験割り当て時の設定永続化が修正された。

Rewindがロールバック時に無視ファイルを保持するようになった。

ターミナルdiffビューでのワイド文字レンダリングが修正された。

git worktree間でのフォルダ信頼の永続化が修正された。

MCP OAuth再認証のアドレス使用中の問題が解決された。

MCPアローリストのnpmスコープサーバーマッチングが修正された。

ローカルMCPトークンブローカーの信頼性が改善された。

BYOK 5MiB超ファイル添付のOpenAI経由での処理が修正された。

gitリポジトリ外での/init提案の抑制が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.60-0)
