# Configuration

各サービスの設定などに付いてのドキュメント

## Network

Docker のネットワーク設定について．

> [!IMPORTANT]
> DB や Redis など複数コンテナからなるようなサービスは固有のネットワークを作成しそこに所属させることを推奨する．\
> 以下に示すネットワークは，所属する必要がある場合に別途アクセスする必要のあるコンテナのみを所属させ
> DB や Redis などアクセスする必要のないコンテナは，所属させるべきではない．

`web-app-network`

- **概要**
  - AWS S3 互換のストレージである MinIO を使用するためのネットワークです．
  - MinIO のネットワーク内 IP アドレスは `172.23.10.1`で固定されています．
  - Bridge network
- **所属するサービス**
  - [MinIO](/docker/minio/compose.yml)
  - [Memos](/docker/memos/compose.yml)
  - [Linkwarden](/docker/linkwarden/compose.yml)
