# README

Deployments には，自宅鯖でセルフホストしているアプリケーショの設定ファイルが置かれています．

## 構成

Deployments で管理されているアプリケーションは以下のようにホスティングされています．\
また，外部へのサービスの公開は[Cloudflare Tunnel](https://www.cloudflare.com/ja-jp/products/tunnel/)を使用しています．

### [docker](./docker/)

- Docker compose を使ってホスティングされています．

## アプリケーション

1.  memos
    - [usememos/memos](https://github.com/usememos/memos)
    - 軽量なメモツールです．
2.  babyrite
    - [m1sk9/babyrite](https://github.com/m1sk9/babyrite)
    - メッセージリンク付きのメッセージを展開してくれる Discord Bot です．
3.  minio
    - [minio/minio](https://github.com/minio/minio)
    - AWS S3 互換のストレージ
4.  miniflux
    - [miniflux/v2](https://github.com/miniflux/v2)
    - RSS Feeder
