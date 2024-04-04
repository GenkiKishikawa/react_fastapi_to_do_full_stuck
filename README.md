# TODO_FastAPI_React

## 概要

FastAPIとReact学習用のレポジトリ 

- [FastAPIレポジトリ](https://gitlab2.vic.co.jp/learning-tsukuba/fastapi/kishikawa/fastapi)
- [Reactレポジトリ](https://gitlab2.vic.co.jp/learning-tsukuba/fastapi/kishikawa/react)

## 開発環境

岸川の開発環境は以下

- WSL2
- Visual Studio Code
- Devcontainer
- Docker version 24.0.7
- Docker Compose version v2.23.3-desktop.2
- node18.16.0(Dockerコンテナ内)
- python3.11(Dockerコンテナ内)

## 開発環境構築

### 1. レポジトリをクローン

```bash
$ git clone --recursive ssh://git@gitlab2.vic.co.jp:2222/learning-tsukuba/fastapi/kishikawa/todo_fastapi_react.git
$ cd todo_fastapi_react
```

### 2. Dockerイメージをビルド

```bash
$ docker compose build --no-cache
```

### 3. Dockerコンテナを起動

Devcontainerを使用する場合は、Visual Studio Codeで右下の`>< WSL: Ubuntu`→`コンテナーで再度開く`をクリックすることでコンテナを起動

```bash
$ docker compose up -d
```

### 4. ブラウザでアクセス

- FastAPI: http://localhost:8000/docs
- React: http://localhost:8001