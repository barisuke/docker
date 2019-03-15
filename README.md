# docker
docker系のファイル保存場所

## XXX-docker-compose.ymlファイルの取扱方法
(XXXはファイルによって異なる)

1.　XXX-docker-compose.ymlがあるディレクトリに移動

2.　以下のコマンドをterminalで実行

```:terminal
$ docker-compose -f XXX-docker-compose.yml up -d
```

3.　stopするときは以下のコマンドをterminalで実行

```:terminal
$ docker-compose -f XXX-docker-compose.yml stop
```

### 例1
```:terminal
$ docker-compose -f mysql-docker-compose.yml up -d

Starting test_mysql_db_1 ... done
```

```
$ docker-compose -f mysql-docker-compose.yml stop
Stopping test_mysql_db_1 ... done
```


# レポジトリ中のファイル一覧

### mysql-docker-compose.yml

mysql環境を構築する

hostOSからmysqlにアクセスする場合は以下を実行する
```
$ mysql -h127.0.0.1 -utest -ptest
```
