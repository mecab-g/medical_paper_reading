# Cousor Tasks Repository

このリポジトリは、Cursor IDEで使用するプロンプトとタスクを保存しています。

## 概要

- Cursor IDEで使用するプロンプトファイルの保存
- 各種タスクの保存と管理
- タスクごとに1つのプロンプトファイルを使用

## ファイル構造

### タスク管理
- 全てのタスクは`memory`ディレクトリで管理
- 各タスクは1つのプロンプトファイルとして保存
例：`memory/medical_paper_reading_task.txt`

### 成果物の保存
- 各タスクの成果物は、対応するプロンプトと同名のディレクトリに保存
- ディレクトリ構造例：
  ```
  memory/
  ├── medical_paper_reading_task.txt     # プロンプトファイル
  ├── medical_paper_reading_task/        # 成果物用ディレクトリ
  │   ├── generated_papers/
  │   └── analysis_results/
  ├── english_question_task.txt          # 別のタスクのプロンプト
  └── english_question_task/             # 対応する成果物ディレクトリ
      ├── questions/
      └── answers/
  ```

### タスク例
- 医学論文読解タスク: `memory/medical_paper_reading_task.txt`
  - 医学論文の読解に関するプロンプト

### プロンプト利用例
- english_question: プロンプトを利用して英語読解問題を作成
  - 医学論文の読解問題と解答を生成
  - 2型糖尿病やがん免疫療法などの専門的な内容に対応

## プロンプトファイルの形式

- 各タスクは1つのテキストファイルとして保存
- ファイル名は内容を反映した分かりやすい名前を使用
- 必要に応じて日本語・英語のプロンプトを含める

## 今後の予定

- タスクの種類を順次追加予定
- プロンプトの最適化と改善 