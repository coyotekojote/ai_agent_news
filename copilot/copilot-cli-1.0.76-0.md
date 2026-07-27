## MCPツールの読み込み高速化

MCPツールが定義スコープのスナップショットからより高速に読み込まれるようになった。プロセス全体およびサーバーごとのキャッシュオプトアウトも追加された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-0)

## Autopilotモードのタスク完了後の動作改善

タスク完了後にAutopilotモードが選択されたままになるようデフォルト動作が変更された。`stayInAutopilot`をfalseに設定することで、タスク完了後にインタラクティブモードに戻ることも可能。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-0)

## コンテキスト制限の早期警告の復元

システムおよびツールのコンテキストが制限に近づいた際の早期警告が復元された。自動コンパクションがブロックされる前にユーザーに通知されるようになった。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-0)

## ワークツリー切り替え後の作業ディレクトリ修正

`/worktree`で新しいワークツリーに切り替えた後、セッションの作業ディレクトリが元のチェックアウトに戻ってしまう問題が修正された。

[参考リンク](https://github.com/github/copilot-cli/releases/tag/v1.0.76-0)
