# LAMP-Docker-Template
DockerとDocker-Composeは予めインストールしてください。

`docker-compose up -d`すると以下のコンテナが立ち上がります。
- PHP8.1
- MariaDB10.6

@envは.envにリネームして、環境変数を適宜変更してください。

## 参考
- [PHP8のLAMP環境をDockerで作ってみる](https://tech.fusic.co.jp/posts/2021-08-12-php8-lamp-on-docker/)
- [Docker Composeを使ってphpからMySQL/MariaDBに接続する環境を作る](https://zenn.dev/qljmssqh/articles/bc2d77262d5e12)
- [PHPのPDOでMariaDB(MySQL)への接続テスト](https://blog.ver001.com/php_pdo_windows/)
