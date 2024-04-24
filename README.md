# Rails7 Boilerplate

1. `docker compose build`
2. `docker compose run --rm web gem install rails`
3. `docker compose run --rm web rails new . -d mysql`  
   アプリケーションの名前を App 以外にしたい場合は、 `-n` オプションで名前を指定する。
4. `config/database.yml` の `default` 内に以下を記述。

```text
username: root
password: password
host: db
```

5. `docker compose up db -d`
6. `docker compose run --rm web rails db:create`
7. `docker compose stop db`
8. `docker compose up -d`
