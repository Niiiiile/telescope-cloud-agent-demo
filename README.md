# telescope-cloud-agent-demo

10kn 統合 AI 基盤の **Phase 1（クラウド実行）** デモ用リポジトリです。

Telescope で「AI に実行させる」判断を付けると、comm-hub が Cursor Cloud Agent をこのリポジトリ上で起動します。Mac 上の Claude Code / monitor ループは不要です。

## 使い方（概要）

1. comm-hub に `CURSOR_API_KEY` を設定
2. Telescope デモプロジェクトの `agentRepository` を `https://github.com/Niiiiile/telescope-cloud-agent-demo` に設定
3. Telescope イベントに `resolutionExecute: true` を付けて判断登録
4. comm-hub cron（5分）または `POST /api/telescope/instructions/run` で起動
5. このリポジトリの `demo/results/latest.md` にサマリがコミットされる

詳細: [remote-tool-for-agent/docs/cloud-agent-demo.md](https://github.com/Niiiiile/remote-tool-for-agent/blob/main/docs/cloud-agent-demo.md)（comm-hub 側ドキュメント）

## ディレクトリ

| パス | 用途 |
|------|------|
| `AGENTS.md` | クラウドエージェント向けの実行規約 |
| `demo/TASK.md` | サンプル指示（手動テスト用） |
| `demo/results/latest.md` | エージェントの実行サマリ出力先 |
