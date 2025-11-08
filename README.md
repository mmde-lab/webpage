# webpage
Hara-Laboratory Official web site.
https://mmde-lab.github.io/webpage/

## ホームページの更新方法

### 方法1: ブラウザ上で編集（簡単・推奨）

1. **GitHubでファイルを編集**
   - 編集したいファイル（例: `web/docs/index.md`）を開く
   - 鉛筆アイコン（Edit this file）をクリック
   - 内容を編集

2. **ブランチを作成してコミット**
   - 下部の "Commit changes" で
   - "Create a new branch for this commit and start a pull request" を選択
   - ブランチ名を入力（例: `update-member-info`）
   - "Propose changes" をクリック

#### **複数ファイルを編集する場合**:
   - 1つ目のファイルで新しいブランチを作成
   - 2つ目以降は同じブランチに直接コミット（"Commit directly to the {branch-name} branch" を選択）

3. **プルリクエストを作成**
   - "Create pull request" をクリック
   - 自動的にプレビューURLが発行されます

4. **確認してマージ**
   - プレビューURLで確認
   - 問題なければ "Merge pull request" をクリック
   - 自動的に本番サイトにデプロイされます

### 方法2: ローカルで編集（高度な編集向け）

1. **リポジトリをクローン**
   ```bash
   git clone git@github.com:mmde-lab/webpage.git
   cd webpage
   ```

2. **ブランチを作成**
   ```bash
   git checkout -b update-homepage
   ```

3. **ファイルを編集**
   - `web/docs/` 内のMarkdownファイルを編集
   - ローカルでプレビュー: `cd web && mkdocs serve`

4. **コミット＆プッシュ**
   ```bash
   git add .
   git commit -m "Update homepage content"
   git push origin update-homepage
   ```

5. **プルリクエストを作成**
   - GitHubでプルリクエストを作成
   - 自動的にプレビューURLが発行されます
   - 確認後、マージするとデプロイされます

## MkDocs Commands - Cheat Sheet

```
# Start Dev-Server
$ cd web/
$ mkdocs serve -a 0.0.0.0:8000
# Open http://localhost:8000/ in your browser
```


## Setup
### 1.Clone Repository
```
# Move to working directory
$ git clone git@github.com:mmde-lab/webpage.git
$ cd webpage
```
### 2.Create Branch
```
$ git checkout -b <ブランチ名>
```
### 3.Edit files

### 4.Docker
```
$ cd webpage/
$ docker-compose build
$ docker-compose up -d
$ docker-compose exec ws /bin/bash
```


### 5.ssh keygen before deploy
```
$ cd ~/.ssh
$ ssh-keygen -t rsa
$ cat id_rsa.pub
$ git config --global user.name "githubのユーザー名"
$ git config --global user.email "email_github"
```
### 6.Add SSH key to GitHub
Open github.com and add your SSH key to your account.
Test SSH connection.
```
$ ssh -T git@github.com
```

### 7.Push
```
$ git add .
$ git commit -m "details of change"
$ git push origin <ブランチ名>
```

### 8.プルリクエストを作成
GitHubでプルリクエストを作成すると、自動的にプレビューURLが発行されます。
確認後、mainブランチにマージすると本番環境に自動デプロイされます。

## Reference
- [mkdocs](https://github.com/mkdocs/mkdocs)
- [mkdocs-material](https://github.com/squidfunk/mkdocs-material)

### git
- [Qitta - GitHubでssh接続する手順~公開鍵・秘密鍵の生成から~](https://qiita.com/shizuma/items/2b2f873a0034839e47ce)

### Python
- [WSL2にpip3をインストール](https://astherier.com/blog/2020/08/install-pip3-on-wsl2/)

```
# Install pip3
$ sudo apt install python3-pip

```
