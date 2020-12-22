# mmde-lab-official-web
Hara-Laboratory Official web site.
https://mmde-lab.github.io/webpage/

## MkDocs Commands - Cheat Sheet
```
# Start Dev-Server (Open http://localhost:8000/)
$ cd web/
$ mkdocs serve -a 0.0.0.0:8000

# Deploy
$ mkdocs gh-deploy
```

## Setup
### Clone Repository
```
# Move to working directory
$ git clone git@github.com:mmde-lab/webpage.git
$ cd webpage
```

### Local (Recomended)
```
$ cd mmde-lab-official-web/
$ pip install -r docker/requirements.txt
```

### Docker (Optional)
```
$ cd mmde-lab-official-web/
$ docker-compose build
$ docker-compose up -d
$ docker-compose exec ws
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