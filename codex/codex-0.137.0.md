## TUI機能の強化

F13〜F24キーバインディング、検索可能メニューでのペースト機能、コンパクトな推論専用ステータス/タイトルアイテムがサポートされた。

TUIのMarkdownレンダリングが改善され、WebリンクがOSC 8メタデータによりクリック可能な状態で維持されるようになった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0)

## エンタープライズ管理機能

月間クレジット制限の可視化とクラウド管理の設定バンドルサポートが追加された。EDUワークスペースとの互換性も含まれる。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0)

## リモートコントロール機能

クライアントペアリングの開始とコントローラー権限管理がapp-server v2 RPCを通じて可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0)

## プラグインの改善

プラグインリストのJSON出力とキャッシュされたリモートカタログの提案が追加され、ワークフロー効率が向上した。

マニフェストの順序保持、ローカル/リモートインストールの重複排除、不正なスキルフィールドのハンドリングが修正された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0)

## Web・画像ツールの拡張

コードモードワークフローでの利用範囲が拡大し、並列スタンドアロンWeb検索の実行が可能になった。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0)

## Multi-Agent v2の改善

スレッド間でのランタイム永続化が実現し、フォローアップの簡素化とスポーンエージェントのメタデータデフォルトが設定された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0)

## セッション管理コマンド

`/archive`コマンドによるセッションアーカイブ機能が追加された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0)

## バグ修正

キャンセルされたプロンプトが出力表示前にドラフト、添付ファイル、コラボレーション設定を復元するようになった。

スラッシュコマンドのフィルタリングとフッターヒントが現在のUI状態に基づいて適切にリセットされるようになった。

macOS起動、Windows SQLiteスタートアップ、スレッド再開、サンドボックスリフレッシュのプラットフォーム安定性が改善された。

権限リクエストでの環境ID伝播と子コマンドのための読み取り可能なCAバンドルエクスポートが修正された。

圧縮ロールアウト、リネームスレッド、パスなしサイドチャット、スタック集約操作のセッション履歴安全性が強化された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0)

## インフラストラクチャの改善

Windows対応のJustfileワークフローとルートフォーマットチェックが追加された。サブモジュール問題解決のためGit CLI統合がCargo操作に導入された。Python SDKホイールがglibc互換ランタイムパッケージで公開された。クレート再編成により`codex-core`の依存関係が削減された。

[参考リンク](https://github.com/openai/codex/releases/tag/rust-v0.137.0)
