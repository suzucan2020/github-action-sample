# アクション

- JavaScriptアクション
- Dockerコンテナアクション

## Dockerコンテナアクション

- リポジトリ内のDockerfile

```yml
runs:
  using: docker
  image: Dockerfile
```

- Docker Hub上のイメージ

```yml
runs:
  using: docker
  image: docker://alpine:3.11
```

- パブリックなDockerレジストリ上のイメージ

```yml
runs:
  using: docker
  image: docker://gcr.io/cloud-builders/gcloud
  args:
    - version
```
