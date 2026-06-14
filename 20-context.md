# コンテキスト駆動開発

## 概要

- コンテキスト駆動開発
- `.context`配下で管理
- プロンプトで明示的に呼ばれたコンテキストファイル以外はRead/Write/Edit不可
- docs/srcの全Read権限を与える
- plan時、Write/Editは不可
- コンテキストファイルの分割単位はWrite/Editするファイル

## フロントマター

```markdown
---
description: コンテキストファイルの説明
status: plan/implement/reviewed/approved/finished
created_by: @vxdora
created_at: 2026/06/05
assumption: @.context/20260503112233.md
---
```

### description

コンテキストファイル概要

### status

コンテキストファイルの状態。

1. planned: 計画段階。実装計画を立てていない状態（概要や背景のみ）ではこのステータス。
2. implement: 調査完了、実装指示書（初期）
3. reviewed: 批判的レビュー完了
4. approved: 人間による承認。
5. finished: 実装完了

### assumption

前提となるコンテキストファイル

## スキル一覧

| スキル名 | 概要 |
| -- | -- |
| /context | コンテキストファイルの作成、計画、分割、レビュー、実装を行う。hooksで管理 |
