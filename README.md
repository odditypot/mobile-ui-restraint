# Mobile UI Restraint

A skill to help your AI agent design phone and iPad screens. Makes the next step clear and keeps useful buttons easy to find. Removes clutter and puts extra technical, legal, and test details in the right place.

AIエージェントに、スマートフォンやiPadの画面づくりを手伝ってもらうためのスキル。次にすることや必要なボタンを分かりやすくし、余計な説明や技術・規約・テストの詳しい話を適切な場所へ整理します。

## English

### Purpose and scope

Use it to build or review app screens, mobile websites, menus, forms, task lists, and dashboards. It helps you choose what belongs on the screen and what can go in Help, Settings, About, or developer notes.

Keep prices, consent, progress, errors, and recovery steps beside the actions they affect. Required notices and useful controls stay available. The aim is to make the screen easier to use, with enough information to make a decision.

Check small phone screens and iPad windows, including when you open the keyboard or resize the window. Also check larger text, screen readers, different languages, and what happens when the app is loading, empty, offline, or has an error. This skill gives your agent guidance. You still need to try the actual screens.

### Install

Put this repository in your agent's skill folder, with `SKILL.md` at `mobile-ui-restraint/SKILL.md`. If your agent reads skills from `~/.agents/skills`, you can use:

```sh
mkdir -p ~/.agents/skills
git clone https://github.com/odditypot/mobile-ui-restraint.git ~/.agents/skills/mobile-ui-restraint
```

Choose an unused folder so you can keep any existing installation. If your agent uses another skill folder, change the destination. Start a new session if your agent loads skills at startup. No extra scripts or packages are needed.

### Use and examples

Show your agent the screen, explain what the user needs to do, and say which devices to check:

> Use mobile-ui-restraint to review this checkout on a small phone and a resizable iPad window. Preserve payment controls, costs, consent, and recovery.

> Use mobile-ui-restraint to redesign this task dashboard. Make status and the next action clear, and check text scaling and keyboard navigation.

For example, a checkout keeps price and consent beside purchase; a task list keeps useful status and the next step; an iPad layout adapts navigation as its window changes. Review actual renders and interactions before delivery. The complete instructions and official platform references are in [SKILL.md](SKILL.md).

## 日本語

### 目的と対象

アプリの画面、モバイルサイト、メニュー、フォーム、タスク一覧、ダッシュボードの作成や見直しに使えます。画面に残す情報と、ヘルプ・設定・About・開発メモへ移す情報を選ぶ手助けをします。

価格、同意、進み具合、エラー、やり直す方法は、関係する操作の近くに置きます。必要な操作や表示義務のある説明は残します。判断に必要な情報を保ちながら、使いやすい画面を目指します。

小さなスマートフォンの画面やiPadのウィンドウで、キーボードを開いたときやサイズを変えたときも確認します。大きな文字、画面読み上げ、別の言語、読み込み中・データなし・オフライン・エラーの表示も扱います。エージェントへの指針として使い、実際の画面や操作も試してください。

### インストール

エージェントが読み込むスキル用ディレクトリに、このリポジトリをcloneします。配置は `mobile-ui-restraint/SKILL.md` です。`~/.agents/skills` を読み込む環境では、上のコマンドを使えます。

既存のスキルを上書きしないよう、未使用の保存先を選んでください。別のスキル用ディレクトリを使う環境では、保存先を変更します。起動時にスキルを読み込む環境では、新しいセッションを開始してください。スクリプトや同梱の依存ファイルはありません。

### 使い方と例

対象の画面、ユーザーの作業、確認する表示サイズを伝えて、スキルの適用を依頼します。

> mobile-ui-restraintを使って、この購入画面を小さなスマートフォンとサイズ変更可能なiPadウィンドウでレビューしてください。支払い操作、費用、同意、エラーからの復帰方法を保ってください。

> mobile-ui-restraintを使って、このタスクダッシュボードを改善してください。状態と次の操作を分かりやすくし、文字サイズの変更とキーボード操作も確認してください。

例えば、購入画面では価格と同意を購入操作の近くに置き、タスク一覧では必要な状態と次の操作を示し、iPadではウィンドウの変化に合わせてナビゲーションを調整します。完成前に実際の表示と操作を検証します。詳細な指示と公式のプラットフォーム資料は [SKILL.md](SKILL.md) にあります。スキル本文は英語です。
