## アダプティブトークンカリキュレーター

より正確なコンテンツサイジングのためのアダプティブトークンカリキュレーターが導入された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26888)

## ダイナミックモデルルーティング

ダイナミックモデル設定使用時にNumericalRouterが有効化されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26929)

## サブエージェント進捗管理の改善

サブエージェントの進捗管理を改善するSubagentState列挙型が導入された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26934)

## SSH経由のエクステンションインストール

SSHリポジトリからのエクステンションインストールが有効化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26274)

## ADK非インタラクティブセッション対応

ADKの非インタラクティブセッションが有効化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26895)

## レガシーセッションの再開機能復旧

レガシーセッションタイプの再開機能が復旧された。

[参考リンク](https://github.com/google-gemini/gemini-cli/pull/26577)

## バグ修正

スナップショッターのモデル設定が修正された。SessionStart systemMessageの重複レンダリングが解消された。ACPモードでnextSpeakerCheckが無効化され、無限思考ループが防止された。NumericalClassifierStrategyのツールターン処理がリファクタリングされ400エラーが解消された。不正なprojects.jsonのハンドリングが追加された。入力プロンプトのガター幅計算が調整された。customIgnoreFilePathsにディレクトリが含まれる場合のEISDIRクラッシュが防止された。Flashクォータ枯渇後の明示的なモデル選択が尊重されるようになった。OAuthフォールバック問題を防ぐためquota_project_idがテレメトリに注入されるようになった。.pakおよび.rpaゲームアーカイブ形式がデフォルトの無視リストに追加された。/resume検索中にEnterキーでセッションを選択できるようになった。VSCodeの現在のファイル実行機能が修正された。ツールプロンプトで静的ツール名が使用されパースの問題が回避されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0-nightly.20260512.gc987b9939)
