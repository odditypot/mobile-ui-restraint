# Mobile UI Restraint

Helps AI agents build cleaner mobile and iPad interfaces.

AIエージェントが、すっきり使いやすいモバイル・iPad画面を作るためのスキル。

## English

### Purpose and scope

Use this skill when building, redesigning, or reviewing phone and iPad screens, mobile web UI, navigation, forms, onboarding, and dashboards. It helps keep the user's current task, next decision, and useful controls clear while preserving the app's workflow and identity.

Restraint means choosing where information belongs. Keep task context, frequent actions, real cost and privacy consequences, progress, and recovery near the decisions they support. Place general explanations in Help, Settings, or About, and engineering details in engineering docs. The goal is usable hierarchy, with enough information to act confidently.

The skill includes phone safe areas and keyboard behavior, iPad window resizing and adaptive navigation, accessibility, localized copy, and loading, empty, error, offline, and confirmation states. It is a design and review guide, not a component library or a substitute for testing real screens.

### Install

Clone this repository into your agent's skill directory, with `SKILL.md` at `mobile-ui-restraint/SKILL.md`. For a runner that discovers skills in `~/.agents/skills`:

```sh
mkdir -p ~/.agents/skills
git clone https://github.com/odditypot/mobile-ui-restraint.git ~/.agents/skills/mobile-ui-restraint
```

Use an unused destination; keep any existing installation until you have compared it. If your runner uses another skill directory, clone there instead. Start a new session if skills are discovered at startup. The package has no scripts or bundled dependencies.

### Use and examples

Ask your agent to apply the skill, supplying the screen, current task, and target viewports:

> Use mobile-ui-restraint to review this checkout on a small phone and a resizable iPad window. Preserve payment controls, costs, consent, and recovery.

> Use mobile-ui-restraint to redesign this task dashboard. Make status and the next action clear, and check text scaling and keyboard navigation.

For example, a checkout keeps price and consent beside purchase; a task list keeps useful status and the next step; an iPad layout adapts navigation as its window changes. Review actual renders and interactions before delivery. The complete instructions and official platform references are in [SKILL.md](SKILL.md).

## 日本語

### 目的と対象

スマートフォン・iPadの画面、モバイルWeb UI、ナビゲーション、フォーム、オンボーディング、ダッシュボードの設計・改善・レビューに使います。アプリの操作フローや個性を保ちながら、ユーザーの現在の作業、次の判断、必要な操作を分かりやすくします。

情報の置き場所を、使う場面に合わせて選びます。作業に必要な文脈、よく使う操作、実際の費用やプライバシーへの影響、進捗、エラーからの復帰方法は、その判断や操作の近くに置きます。一般的な説明はヘルプ・設定・Aboutへ、実装の詳細は開発ドキュメントへ整理します。安心して操作できる情報量と、明確な優先順位を目指します。

スマートフォンのセーフエリアやキーボード、iPadのウィンドウサイズ変更とナビゲーション、アクセシビリティ、多言語の文言、読み込み中・空・エラー・オフライン・確認の状態も扱います。設計とレビューのためのガイドであり、コンポーネント集ではありません。実際の画面や操作の検証と併せて使います。

### インストール

エージェントが読み込むスキル用ディレクトリに、このリポジトリをcloneします。配置は `mobile-ui-restraint/SKILL.md` です。`~/.agents/skills` を読み込む環境では、上のコマンドを使えます。

既存のスキルを上書きしないよう、未使用の保存先を選んでください。別のスキル用ディレクトリを使う環境では、保存先を変更します。起動時にスキルを読み込む環境では、新しいセッションを開始してください。スクリプトや同梱の依存ファイルはありません。

### 使い方と例

対象の画面、ユーザーの作業、確認する表示サイズを伝えて、スキルの適用を依頼します。

> mobile-ui-restraintを使って、この購入画面を小さなスマートフォンとサイズ変更可能なiPadウィンドウでレビューしてください。支払い操作、費用、同意、エラーからの復帰方法を保ってください。

> mobile-ui-restraintを使って、このタスクダッシュボードを改善してください。状態と次の操作を分かりやすくし、文字サイズの変更とキーボード操作も確認してください。

例えば、購入画面では価格と同意を購入操作の近くに置き、タスク一覧では必要な状態と次の操作を示し、iPadではウィンドウの変化に合わせてナビゲーションを調整します。完成前に実際の表示と操作を検証します。詳細な指示と公式のプラットフォーム資料は [SKILL.md](SKILL.md) にあります。スキル本文は英語です。
