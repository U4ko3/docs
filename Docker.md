# 🐳 Docker コマンド集

## 基本操作

| コマンド         | 説明                         |
| ---------------- | ---------------------------- |
| `docker version` | Dockerのバージョン情報を表示 |
| `docker info`    | Dockerのシステム情報を表示   |
| `docker help`    | ヘルプを表示                 |

---

## 📦 イメージ操作

| コマンド                   | 説明                                      |
| -------------------------- | ----------------------------------------- |
| `docker pull <image>`      | イメージを取得（例: `docker pull nginx`） |
| `docker build -t <name> .` | Dockerfileからイメージを作成              |
| `docker images`            | ローカルにあるイメージ一覧を表示          |
| `docker rmi <image>`       | イメージを削除                            |

---

## 🚀 コンテナ操作

| コマンド                           | 説明                                     |
| ---------------------------------- | ---------------------------------------- |
| `docker run <image>`               | コンテナを起動（例: `docker run nginx`） |
| `docker run -d <image>`            | バックグラウンドで起動                   |
| `docker run -it <image> /bin/bash` | 対話型で起動                             |
| `docker ps`                        | 起動中のコンテナ一覧を表示               |
| `docker ps -a`                     | 全コンテナ一覧（停止中含む）             |
| `docker stop <container>`          | コンテナを停止                           |
| `docker start <container>`         | コンテナを開始                           |
| `docker restart <container>`       | コンテナを再起動                         |
| `docker rm <container>`            | コンテナを削除                           |

---

## 🛠 コンテナ内操作

| コマンド                                | 説明                         |
| --------------------------------------- | ---------------------------- |
| `docker exec -it <container> /bin/bash` | コンテナに入る               |
| `docker logs <container>`               | コンテナのログを表示         |
| `docker cp <container>:<path> <local>`  | コンテナからファイルをコピー |
| `docker inspect <container>`            | コンテナの詳細情報を表示     |

---

## 🧹 クリーンアップ

| コマンド                 | 説明                     |
| ------------------------ | ------------------------ |
| `docker system prune`    | 未使用のデータを一括削除 |
| `docker image prune`     | 未使用のイメージを削除   |
| `docker container prune` | 停止中のコンテナを削除   |

---

## 🧱 Docker Compose

| コマンド               | 説明                   |
| ---------------------- | ---------------------- |
| `docker-compose up`    | コンテナ群を起動       |
| `docker-compose down`  | コンテナ群を停止・削除 |
| `docker-compose build` | イメージをビルド       |
| `docker-compose ps`    | コンテナの状態を確認   |
