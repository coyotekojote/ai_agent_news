## フォーカスビュー（VSCode）

チャットメニューからトグルできるフォーカスビューが追加された。ツールのアクティビティをターンごとの展開可能なサマリーの背後に隠し、実行中のツールインジケーターをライブ表示する。`Ctrl+Alt+F`または「Claude Code: Toggle Focus view」コマンドで切り替え可能。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サンドボックスの資格情報ファイルマスキング（Linux/WSL）

サンドボックスの資格情報ファイルに`mode: "mask"`が追加された。サンドボックス内のコマンドはセンチネルコピー（ファイル全体または`extract`正規表現でキャプチャされたスパン）を読み取り、サンドボックスプロキシが送信時に実際の値を代入する。macOSではファイルマスキングは`deny`にフォールバックする。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインバリデーション警告

`claude plugin validate`にClaude Desktopのマネージドマーケットプレイス同期でマーケットプレイス名またはプラグイン名が拒否される場合の警告が追加された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プロンプト監査サブコマンド

`claude-api`スキルに`prompt-audit`サブコマンドが追加された。プロンプトやツールの説明が古いモデル向けに書かれたパターンを監査する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セキュリティ修正：Bashツールの権限チェックバイパス

zshが`[[ ]]`正規表現条件式内で隠しコマンドを実行できる権限チェックバイパスが修正された。影響を受けるコマンドは権限の確認を求めるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セキュリティ修正：PowerShellの権限チェック

Windows上でクォート文字を含むパスの処理が修正された。このようなパスは承認を求めるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## シンキングトグルの修正

シンキングオフで開始されたセッションの残りでシンキングトグルが効果を持たない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## MCPサーバー接続の修正

接続中にMCPサーバーを無効にしても静かに元に戻らなくなった。また、printモード（`-p`）で`--mcp-config`からのMCPサーバーが最初のターン前に接続しない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ファイルメンションの修正

`@`でメンションされたファイルがEscキーでプロンプトを撤回して再送信した際に静かにドロップされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## SDK MCPツールのクラッシュ修正

組み込みオブジェクトプロパティ（例：`constructor`）と同名のSDK MCPツールに対するAPIリクエスト準備時のクラッシュが修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## WebSearchの修正

シンキングが無効な場合にeffort `xhigh`/`max`でWebSearchが400エラーで失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## サンドボックス内の大容量アップロード修正

サンドボックスプロキシを経由した大容量アップロードがTLSエラーで失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 利用制限メッセージの修正

TeamおよびEnterpriseの利用制限メッセージが、個人の利用制限ではなく組織の月間制限を誤って表示する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bedrock AWS SSO認証の修正

Windows上でストレイ`HOME`環境変数がある場合に、デスクトップ管理セッションでAWS SSO名前付きプロファイルによるBedrock認証が失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 環境変数ハンドリングの修正

`CLAUDE_CODE_RESUME_INTERRUPTED_TURN=0`が中断ターンの自動再開を無効化しない問題が修正された。偽値が適切に扱われるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## トークンリフレッシュ競合状態の修正

スリープからの復帰時に2つのClaude Codeプロセスが同時にMCPコネクタまたはWIF OAuthトークンをリフレッシュしてしまう競合状態が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッション名同期の修正

Claude Code DesktopまたはClaude.aiからセッション名を変更してもCLIのセッション名が更新されない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## ターミナル専用ビルトインの修正

ターミナル専用ビルトイン（例：`/help`、`/feedback`）と同名のプラグインおよび組織提供スキルが非インタラクティブセッションで呼び出せない問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 通知の永続化修正

プラグインがリロードされた後も「Plugins changed」通知がクリアされずに残る問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Vimモードのヤンクレジスタ修正

ダイアログ、履歴検索、トランスクリプトビューでヤンクレジスタが静かに空にされる問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Vimモードの空プロンプトへのアンドゥ修正

空のプロンプトまでアンドゥした場合、エージェントビューに戻る前に「← をもう一度押して確認」が表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Google Vertex AIのツールサーチ再有効化

Claude 4.5世代以降のモデルでGoogle Vertex AIのツールサーチが再有効化された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## オートモードの権限チェック最適化

並列ツール呼び出しの権限チェックがキャッシュ効率化された。チェック保留中のモード切り替えが、古い結果の適用ではなく確実にプロンプトするようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プロンプトキャッシュコストの削減

オートモード権限チェックで会話プレフィックスのキャッシュを再利用することにより、プロンプトキャッシュコストが削減された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 統計パネルの改善

トークン合計にキャッシュトークンがカウントされるようになり、入力、出力、キャッシュ読み取り、キャッシュ書き込みの内訳が表示されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Windowsの起動パフォーマンス向上

プロセス作成時間がPowerShellの起動ではなくネイティブkernel32呼び出しで読み取られるようになった。PowerShell.exeをゲートするエンドポイントセキュリティツールがプロンプトしなくなった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## バックグラウンドセッションの改善

作業を保存するためにコミットとプッシュを行い、タスクが要求した場合のみドラフトPRを開くように変更された。`CLAUDE.md`のgit指示に従い、常に作業の場所を報告して終了するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグインインストールの改善

`/plugin install`が古いマーケットプレイスカタログをリフレッシュしてリトライしてからプラグインが見つからないと報告するように変更された。安全な場合、`/plugin`からインストールされたプラグインは即座にアクティブになるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## セッションフォークの改善

`/fork`でフォークされたセッションが、元のセッションのチェックアウトで作業する代わりに独自のワークツリーを作成するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Fastモードの改善

セッション中に使用クレジットが尽きた場合、静かに失敗するのではなくストリーム上で報告されるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)
