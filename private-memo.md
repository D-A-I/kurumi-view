# kurumi-view

## 予定

1. `kurumi-crawler`の稼働
1. 導入するpackageを再検討
    - prettier
    - tslint -> eslint
1. .dockerignore追加
1. 画面レイアウトを設計

## メモ

- bashで`node:15.3.0-buster-slim`をビルドする

```bash
docker image build \
-f .devcontainer/Dockerfile \
-t test .
```

- `node:15.3.0-buster-slim`に、bashでアクセスする

```bash
docker container run \
-it \
--name test \
-h test \
node:15.3.0-buster-slim /bin/bash
```
