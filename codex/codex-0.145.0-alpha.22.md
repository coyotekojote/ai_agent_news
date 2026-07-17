## 親所有サブエージェントスレッドのTUI読み取り専用化

マルチエージェントV2で生成されたスレッドに`Thread.canAcceptDirectInput`機能が追加された。親が制御するスレッドはTUIで閲覧専用として表示され、下書き、キュー入力、ローカルナビゲーションは保持される。

[参考リンク](https://github.com/openai/codex/pull/33841)

## インストール済みアプリのランタイム状態読み取りAPI追加

新しい`app/installed`エンドポイントが追加され、名前、`enabled`、`callable`状態を含むコネクターランタイム情報を取得できるようになった。スレッド固有の設定評価と強制スナップショット更新をサポート。

[参考リンク](https://github.com/openai/codex/pull/33843)

## 使用量制限リセット前の確認ポップアップ追加

使用量制限リセットの引き換え前に確認ポップアップが表示されるようになった（デフォルトは「No, go back」）。バックエンド提供のリセットタイトル/説明が表示され、重複/古いイベントが処理される。

[参考リンク](https://github.com/openai/codex/pull/33845)

## Web検索結果ペイロードサイズのテレメトリ記録

Web検索結果のシリアライズされたサイズが`codex.web_search.results.payload_bytes`ヒストグラムにテレメトリとして記録されるようになった。

[参考リンク](https://github.com/openai/codex/pull/33851)

## バッチ実行者機能ディスカバリーの追加

新しい`capabilityRoots/discoverV1` exec-server RPCが追加され、機能ルートをスキャンしてプラグインマニフェスト、設定ファイル、スキル命令、メタデータを1回のバウンドリクエストで具現化できるようになった。`executor_capability_discovery`フィーチャーフラグでオプトイン。

[参考リンク](https://github.com/openai/codex/pull/33852)

## リアルタイムトランスクリプトテールフラッシュ委任のタグ付け

リアルタイム委任ペイロードにトランスクリプトフラッシュ時の`<source>transcript_tail_flush</source>`タグが追加された。既存のハンドオフペイロードは変更なし。

[参考リンク](https://github.com/openai/codex/pull/33855)

## リアルタイムV3 Codexハンドオフ出力のストリーミング

エージェントメッセージの更新が完了を待つ代わりに200msインターバルでストリーミングされるようになった。最終出力に「Agent Final Message」ラベルが追加され、切り捨て時にコンテンツの先頭と末尾が保持される。

[参考リンク](https://github.com/openai/codex/pull/33856)

## 空のマルチエージェントモードメッセージの抑制

空の`multi_agent_mode_hint_text`が命令なしとして扱われるようになった。初期ターンやセッション再開時の空メッセージが防止される。

[参考リンク](https://github.com/openai/codex/pull/33862)

## セッションインポートエラータイプの詳細レポート

セッションインポート失敗に対して`sub_error_type`カテゴリ（検出、準備、設定、スレッドストレージ、台帳更新エラー）が追加された。

[参考リンク](https://github.com/openai/codex/pull/33863)

## コードモードのyieldタイムアウトに猶予期間追加

10秒以上の`exec`および`wait`のyieldタイムアウトに1秒の猶予期間が追加された。デッドラインの直後にネストされたツール呼び出しが完了した場合に不正にyieldレスポンスがトリガーされる問題が修正された。

[参考リンク](https://github.com/openai/codex/pull/33867)

## マネージドBedrockログアウトテストアサーションの修正

テストアサーションがalpha.20のenum-to-boolean変更に合わせて`uses_codex_managed_credentials`を使用するように更新された。

[参考リンク](https://github.com/openai/codex/pull/33848)

## zshフォーク拒否テストの実行時間延長

フォーク拒否テストのシェルコマンドタイムアウトが5秒から20秒に延長された。

[参考リンク](https://github.com/openai/codex/pull/33842)

## コアテストのシェルおよびロールアウト永続化からの分離

`test_codex()`でデフォルトで`ShellSnapshot`が無効化された。各承認シナリオに専用のインメモリスレッドストアが付与された。

[参考リンク](https://github.com/openai/codex/pull/33858)

## execサーバー間のワークスペース書き込み分離テスト追加

異なるワークスペースルートを持つ2つのexecサーバー環境が互いのワークスペースに書き込めないことを検証するUnix統合テストが追加された。

[参考リンク](https://github.com/openai/codex/pull/33861)

## フィーチャーテストの動作焦点化

フィーチャーレジストリメタデータを再述するだけのテストが削除された。動作契約（エイリアス、依存関係正規化、非推奨設定）のカバレッジは保持。

[参考リンク](https://github.com/openai/codex/pull/33864)

## 冗長なツールディスパッチラッパーの削除

`ToolRegistry::dispatch_any`パススルーメソッドが廃止された。テストが`dispatch_any_with_terminal_outcome`を直接呼び出すようになった。

[参考リンク](https://github.com/openai/codex/pull/33866)

## 古い無視されたコアテストの削除

無視されていたexplorerロールテストと、タイムアウトキャッピングおよび完了済みセッションクリーンアップの2つの無視された統合execテストが削除された。

[参考リンク](https://github.com/openai/codex/pull/33868)

## 冗長なborrowed行ラッピングヘルパーの削除

`word_wrap_lines_borrowed`が削除され、汎用の`word_wrap_lines` APIに統合された。

[参考リンク](https://github.com/openai/codex/pull/33870)
