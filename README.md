# armRails6Envについて

## 詳細
- Ruby2.6.3、Ruby2.7.5でのRails6の動作を比較したものです。
- どちらの環境でも`./app`フォルダにプロジェクトが生成されます。

## 使い方
1. リポジトリをcloneする
2. `docker compose build`を行いビルドする
3. `docker compose up -d`でコンテナを起動する
4. コンテナ内に接続する
  - `docker exec -it ruby26 bash`でRuby2.6.3の環境に接続する
  - `docker exec -it ruby27 bash`でRuby2.7.5の環境に接続する
5. `rails new`で検証する

## 注意点
- `docker compose build`に10分以上時間がかかる場合があります。