# Python-dev
* コンテナの起動
```
$ docker-compose up -d --build
```

* FastAPIのインストール
```
$ docker exec -it python3 pip install fastapi uvicorn
```

* FastAPIを実行
```
$ docker exec -it python3 zsh -c "cd src && uvicorn main:app --host 0.0.0.0 --reload"
```

* 以下URLにアクセス
  * http://localhost:8000/
  * http://localhost:8000/items/5?q=somequery
  * http://localhost:8000/docs