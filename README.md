# webpage
Hara-Laboratory Official web site.
https://mmde-lab.github.io/webpage/

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
### 8.Deploy
```
$ cd web
$ mkdocs gh-deploy
```

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
