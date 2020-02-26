# Hello Strapi and Heroku (PostgreSQL)
Strapi を Heroku にデプロイするサンプルです。
データベースには、PostgreSQL を使います。

## Heroku の設定
環境変数には、`heroku config`から得たデータベースの情報を設定してください。
```
heroku login
heroku create
heroku addons:create heroku-postgresql:hobby-dev
heroku config
heroku config:set DATABASE_USERNAME=
heroku config:set DATABASE_PASSWORD=
heroku config:set DATABASE_HOST=
heroku config:set DATABASE_PORT=
heroku config:set DATABASE_NAME=
git push heroku master
```

