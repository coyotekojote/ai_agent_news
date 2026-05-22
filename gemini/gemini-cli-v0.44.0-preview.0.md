## エージェント登録の優先順位変更

エージェント登録がfirst-wins方式に変更され、プロジェクトが優先されるようになった。`adk.agentSessionSubagentEnabled`フラグによるエージェントセッション設定が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-preview.0)

## LocalSessionInvocationおよびRemoteSessionInvocation

`LocalSessionInvocation`および`RemoteSessionInvocation`が導入され、AgentSessionの呼び出しがagent-toolに統合された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-preview.0)

## Autoモードの統合

複数のAutoモードが単一のAutoモードに統合された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-preview.0)

## agent-tuiおよびtui-testerスキルの追加

`agent-tui`および`tui-tester`スキルが追加され、TUI関連のエージェント機能が拡張された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-preview.0)

## Sublime TextおよびEmacsクライアントエディタのサポート

Sublime TextとEmacsクライアントエディタのサポートが追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-preview.0)

## RAGスニペットのローカルログ公開

RAGスニペットがデバッグ用にローカルログファイルに公開されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-preview.0)

## content-utilsのコンパイル時網羅性チェック

コアのcontent-utilsにコンパイル時の網羅性チェックが強制されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-preview.0)

## PowerShell Core優先設定

WindowsでレガシーのWindows PowerShell 5.1よりもPowerShell Core（pwsh.exe）が優先されるようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-preview.0)

## 非インタラクティブモードでのMCPサーバー設定対応

非インタラクティブモードでもMCPサーバーの設定が可能になった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-preview.0)

## バグ修正・改善

OAuthリフレッシュトークンのローテーションおよび取得時の保持が改善された。キーチェーン認証がセッション一覧表示と非インタラクティブモードで許可されるようになった。パストラバーサル脆弱性がカスタムコマンドファイルインジェクションで防止された。`NO_PROXY`環境変数がMCPサーバーおよびグローバルfetchディスパッチャーで尊重されるようになった。PTY環境（WSL2、Kitty、Alacritty）でのSIGHUP終了が防止された。Windowsでのインタラクティブシェルの矢印キーナビゲーション問題が解消された。MCPツールのnullable配列型の処理が修正された。proxy-agentのESMバンドルエクスポートが保持されるようになった。シェルテキスト出力のスロットリングとライブUIバッファの制限が追加された。セッション間のスナップショットリカバリが改善された。ファイルストレージマイグレーションの例外処理が改善された。テーブルカラム幅のクランプが改善された。gemini-3.1モデルのエイリアスとthinking設定が追加された。枯渇クォータモデルに対する安定したフォールバックルーティングが確保された。AUTO_EDITモードでのシェルリダイレクションが自動承認されるようになった。PolicyEngineがACPセッションに統合されデッドロックが防止された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.44.0-preview.0)
