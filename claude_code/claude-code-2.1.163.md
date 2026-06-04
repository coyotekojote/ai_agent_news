## 管理設定の強化

`requiredMinimumVersion`と`requiredMaximumVersion`の管理設定が追加された。Claude Codeのバージョンが許可範囲外の場合、起動を拒否し承認済みバージョンへの案内を表示する。

[参考リンク](https://code.claude.com/docs/en/changelog)

## プラグイン管理コマンド

`/plugin list`コマンドが追加され、インストール済みプラグインの一覧表示が可能になった。`--enabled`/`--disabled`フィルタに対応。

[参考リンク](https://code.claude.com/docs/en/changelog)

## /btwコマンドの改善

`/btw`にコピー用ショートカット「c to copy」が追加され、生のMarkdown回答をクリップボードにコピーできるようになった。他の場所にペーストする際にフォーマットが保持される。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Hooks・Skills・MCPの改善

StopフックとSubagentStopフックが`hookSpecificOutput.additionalContext`を返せるようになり、フックエラーとしてラベル付けされずにClaudeへフィードバックを提供しターンを継続できるようになった。

Skillsにおいて`\$`エスケープ構文が追加され、コマンドボディ内で数字の前にリテラル`$`を含めることが可能になった。

stdio MCPサーバーが`--resume`時にフックやBashと同じ`CLAUDE_CODE_SESSION_ID`を受け取るようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## claude -pの修正

`claude -p`がバックグラウンドコマンドが終了しない場合に最終結果後に永久にハングする問題が修正された。stdinが閉じた後約5秒でバックグラウンドシェルが停止されるようになった。

`claude -p`がBedrock/Vertex/Foundry使用時に`CI=true`でAnthhropic APIキーが未設定の場合に「ANTHROPIC_API_KEY required」で失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## Bashコマンドの修正

bazelやEDR保護されたGoワークフローでBashコマンドが失敗する問題が修正された。`$TMPDIR`がサンドボックスコマンドだけでなくすべてのコマンドに対して`/tmp/claude-{uid}`にオーバーライドされていた（2.1.154でのリグレッション）。

WindowsでBashコマンドがセッションenvディレクトリに読み取り専用属性がある場合やOneDrive内にある場合に「EEXIST: file already exists」で失敗する問題が修正された。

[参考リンク](https://code.claude.com/docs/en/changelog)

## 権限・セキュリティの修正

org管理の権限ルールが、新規設定ディレクトリでの起動中に管理設定のフェッチが完了した場合にセッション全体に適用されない問題が修正された。

deny/askルールでホームディレクトリパス（例：`Read(~/Desktop/**)`）を指定した場合、`$HOME`経由でパスを参照するBashコマンドがブロックされない問題が修正された。

フック条件`if: "Bash(...)"`が`$()`や`$VAR`を含むすべてのBashコマンドで発火する問題が修正され、サブシェルやバッククォート内のコマンドに対してもパターンマッチが行われるようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## エージェント・セッション管理の修正

`claude agents`でバックグラウンドセッションがClaude Codeアップデート後に再アタッチした際に実行中のバックグラウンドタスクを失う問題が修正された。

エージェントビューからEscで終了する際のターミナルのずれと数秒間のハングが修正された。

バックグラウンドエージェントセッションがバックグラウンドで新バージョンに更新されるようになり、アップデート後にセッションを開く際にコールドリスタートを待つ必要がなくなった。

`claude agents`のステートグループビューからのディスパッチが、エージェントビューを開いたディレクトリでセッションを開始するようになった。

[参考リンク](https://code.claude.com/docs/en/changelog)

## UI/UXの修正

デスクトップアプリでバックグラウンドタスクチップのStopをクリックした際、基盤プロセスが既に終了している場合にチップがクリアされない問題が修正された。

ペースト操作の終了マーカーがターミナルによってドロップされた場合にキーボード入力が恒久的に無応答になる問題が修正された。

/mcpや/pluginsなどのパネルダイアログを閉じた後にトランスクリプトに残る「(no content)」行が修正された。

サブスクリプション切り替えの提案がトーストではなくスタートアップアナウンスメントスロットに表示されるようになった。

/メニューの組み込みコマンドとスキルの説明がより明確になった。

[参考リンク](https://code.claude.com/docs/en/changelog)
