## コードレビュー自動修正機能

`/code-review --fix`でレビュー結果をワーキングツリーに自動適用できるようになった。再利用・簡略化・効率性の改善提案が反映される。`/simplify`が`/code-review --fix`を呼び出すようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## スキルのdisallowed-tools設定

スキルおよびスラッシュコマンドのフロントマターに`disallowed-tools`を設定し、スキル実行中にモデルから特定のツールを除外できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /reload-skillsコマンドの追加

`/reload-skills`コマンドが追加され、セッションを再起動せずにスキルディレクトリを再スキャンできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## SessionStartフックの拡張

`SessionStart`フックが`reloadSkills: true`を返すことで、フックによってインストールされたスキルを同一セッション内で利用可能にできるようになった。また、`hookSpecificOutput.sessionTitle`で起動時および再開時にセッションタイトルを設定できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MessageDisplayフックイベントの追加

`MessageDisplay`フックイベントが追加され、フックがアシスタントメッセージの表示テキストを変換または非表示にできるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインマーケットプレイスの管理設定

`pluginSuggestionMarketplaces`マネージド設定が追加され、管理者がコンテキスト対応のヒントで提案されるプラグインの組織マーケットプレイスを許可リストに追加できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインマーケットプレイスのスコープ指定

`claude plugin marketplace remove`に`--scope user|project|local`オプションが追加され、`marketplace add`、`install`、`uninstall`と対称的に操作できるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## フォールバックモデルの動作改善

プライマリモデルが見つからない場合、リクエストごとに失敗する代わりに、セッション全体で`--fallback-model`に自動切り替えされるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Autoモードの同意不要化

Autoモードがオプトイン同意なしで利用可能になった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Vimモードの改善

NORMALモードで`/`キーが逆方向の履歴検索（Ctrl+Rと同等）を開くようになり、bash/zshのvi-modeと一致する動作となった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /usageコマンドの拡張

`/usage`の内訳に大きなセッションファイルが含まれるようになった。ファイルはストリーミング読み取りでスキャンされ、メモリ使用量が一定に保たれる。

[参考リンク](https://code.claude.com/docs/en/changelog)

## シンキング表示の改善

折りたたみグループ内のシンキングサマリーが最低3秒間表示され、Markdownとしてレンダリングされ、10行に制限されるようになった（`Ctrl+O`で完全なシンキングを表示）。フルスクリーンモードでは「Thinking for Ns」インジケーターがモデル思考中にリアルタイムでカウントアップし、中断時も値が保持される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ワークフロー表示の簡略化

Workflowツールのインライン進捗表示が簡略化され、ライブエージェント数がプロンプト下の永続的なワークフローステータス行にのみ表示されるようになった。レスポンス後タイマーで、バックグラウンドエージェントやワークフローの完了待機メッセージが表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## OpenTelemetryメトリクス属性の追加

セッションのエントリポイントがOpenTelemetryメトリクス属性（`app.entrypoint`）として追加された（`OTEL_METRICS_INCLUDE_ENTRYPOINT=true`でオプトイン）。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バグ修正・改善

ターミナルスタイリング、ローディングスピナー、フォーカスモード、ツール結果、Markdownテーブル、プラグイン重複排除、MCPサーバー、リモートコントロールなどに関する複数のバグ修正が行われた。

[参考リンク](https://code.claude.com/docs/en/changelog)
