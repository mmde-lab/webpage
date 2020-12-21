# mmde-lab-official-web
Hara-Laboratory Official web site.

## Web Site
https://mmde-lab.github.io/mmde-lab-official-web/

---
## MkDocs Commands - Cheat Sheet
```
# Start Dev-Server (Open http://localhost:8000/)
$ mkdocs serve -a 0.0.0.0:8000

# Deploy
$ mkdocs gh-deploy
```

## Setup
### Local (Recomended)
```
$ cd mmde-lab-official-web/
$ pip install -r docker/requirements.txt
```

### Docker 
```
$ cd mmde-lab-official-web/
$ docker-compose build
$ docker-compose up -d
$ docker-compose exec ws
```

## Reference
- [mkdocs](https://github.com/mkdocs/mkdocs)
- [mkdocs-material](https://github.com/squidfunk/mkdocs-material)
