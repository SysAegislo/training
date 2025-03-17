# training

## 📌 リポジトリの概要
このリポジトリは、研修課題を管理するためのものです。<br>
研修の一環として、各メンバーが課題を進め、成果物を提出する際に使用します。


## 📖 内容
- **課題**：`docs/` ディレクトリ内に研修課題とコーディング規約を格納
- **提出用フォルダ**：`submissions/` フォルダに、各メンバーの成果物を格納


## 🚀 使い方
### 1. リポジトリのクローン
まずはローカルにリポジトリをクローンします：
```bash
git clone git@github.com:SysAegislo/training.git
cd training
```
### 2. 課題の確認
docs/ フォルダ内の課題説明を確認し、コーディング規約に基づいて課題に取り組みます。<br>
その際にTrelloに課題ごとのチケットを作成してください。<br>
(ex.【研修課題】〇〇 フロントエンド課題１)

### 3. 成果物の提出
各自の成果物を submissions/ フォルダ内の自分のディレクトリ（submissions/yourname/）に格納し、プルリクエストを作成してください。

```bash
git checkout -b feature/yourname-task
git add submissions/yourname/
git commit -m "yourname - 課題X 提出"
git push origin feature/yourname-task
```
その後、GitHub 上で Pull Request を作成してください。<br>
その後はチャットワークでレビュー依頼とTrelloのチケットの更新をしてください。<br>

## 📌 ルール・注意事項
- 課題ごとに専用のブランチを作成 してください。
- main ブランチには直接 push しない でください。
