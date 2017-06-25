
## 環境構築手順

### データベース作成

```sh
$ sh ./create-local-mysql-db.sh
```

### マイグレーション

```sh
$ sbt flywayClean
$ sbt flywayMigrate
```

### 動作確認

```sh
$ sbt clean compile
$ sbt run
```


