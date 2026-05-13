## 音声モード対応

マイクアイコンと波形アニメーションによる音声モードが追加された。音声文字起こしがカーソル位置に挿入されるようになり、Gemini Liveバックエンドに対するプライバシー/コンプライアンス警告UIも導入された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0)

## コマンド・スキルの追加

`/bug-memory`コマンド（ヒープスナップショット自動取得機能付き）が追加された。`/exit`コマンドに`--delete`フラグが追加されセッション削除が可能になった。`/commands list`サブコマンドが導入された。`delete`が`/extensions uninstall`のエイリアスとして使用可能になった。geminiロボットへのメンション機能が追加された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0)

## Gemma 4モデルのデフォルト有効化

Gemini API経由でGemma 4モデルがデフォルトで有効化された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0)

## 設定・環境の改善

`ignoreLocalEnv`設定および`--ignore-env`フラグが追加された。サブディレクトリやワークツリーでのブランチインジケーター更新が改善された。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0)

## APIタイムアウトの短縮

デフォルトのAPIタイムアウトが60秒に短縮され、undiciによるリトライがサポートされた。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0)

## バグ修正

自動更新が安定性の低いチャネルに切り替わる問題が修正された。DECKPAMキーパッドのEnterシーケンス処理が修正された。Escapeキーで入力バッファがクリアされない問題が修正された。readStdinのサイズ制限のバイト長計算が修正された。InvalidStreamイベント発生時の「System: Please continue」誤挿入が修正された。`ERR_STREAM_PREMATURE_CLOSE`のエラーハンドリングが改善された。ツール承認のレースコンディションが修正された。`exit_plan_mode`がシェル経由で起動できる問題が修正された。拡張機能ベースのMCPクライアント切断が適切に処理されるようになった。APIキーバリデーションロジックが修正された。設定ダイアログのmaxHeight調整によるレンダリングが改善された。サブエージェントがアクティブな承認モードを認識するようになった。

[参考リンク](https://github.com/google-gemini/gemini-cli/releases/tag/v0.42.0)
