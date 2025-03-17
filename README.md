# training

## 📌 リポジトリの概要
このリポジトリは、研修課題を管理するためのものです。<br>
研修の一環として、各メンバーが課題を進め、成果物を提出する際に使用します。


## 📖 内容
- **課題**：`docs/` ディレクトリ内に研修課題を格納
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


# 🚀 研修課題用 コーディング規約

## 1️⃣ **フォーマット & スタイル**

### ✅ **インデント**
- **タブ1つ**

```python
# ✅ OK (タブ1つ)
def hello_world():
    print("Hello, World!")

# ❌ NG (スペース2つ)
def hello_world():
  print("Hello, World!")
```

### ✅ ** 1行の長さ**
- 80～100文字 以内にする（長すぎると可読性が低下）
- 長くなる場合は 改行 する


### ✅ **変数・関数名**
- Pythonはスネークケースを使用
- JavaScriptはキャメルケースを使用
- 定数はすべて大文字（UPPER_CASE）にする

python
```python
# ✅ OK（スネークケース）
user_name = "Caesar"
def get_user_name():
    return user_name

# ❌ NG（キャメルケースはPythonでは使わない）
userName = "Caesar"
def GetUserName():
    return userName
```
javascript
```javascript
// ✅ OK（キャメルケース）
let userName = "Caesar";
function getUserName() {
    return userName;
}

// ❌ NG（スネークケースはJavaScriptでは使わない）
let user_name = "Caesar";
function get_user_name() {
    return userName;
}
```
### ✅ **ファイル名**
- Python: スネークケース (user_info.py)
- JavaScript: キャメルケース (userInfo.js)

## 2️⃣ **コメントのルール**
### ✅ **コメントの書き方**
- 必要な箇所に簡潔なコメントを入れる
- 関数やクラスには Docstring（Python）または JSDoc（JavaScript）を使う
- コードの意図がわかりやすいように説明する

python
```python
def add_numbers(a, b):
    """
    2つの数を足し算する関数
    :param a: int
    :param b: int
    :return: int
    """
    return a + b
```
javascript
```javascript
/**
 * 2つの数を足し算する関数
 * @param {number} a 
 * @param {number} b 
 * @returns {number}
 */
function addNumbers(a, b) {
    return a + b;
}
```

## 3️⃣ **Gitのコミットメッセージ**
- 50文字以内で簡潔に書く
- 英語なら現在形（Add, Fix, Update） を使う
- 日本語なら「◯◯を追加」「バグ修正」などシンプルに


```bash
# ✅ OK
git commit -m "Add user login function"
git commit -m "Fix bug in payment processing"
git commit -m "Update README with coding style"

# ❌ NG
git commit -m "修正"
git commit -m "とりあえず変更"
git commit -m "aaaa"

```