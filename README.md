# epoll勉強用コード

https://qiita.com/legokichi/items/7b16ab18d66485ace1c6 を参考に実装

# このレポジトリで出来るようになること

- epollのことが少しわかる

# How To Use

```bash
cd /to/this/repository
docker build -t rust-env . # dockerビルド (rust-envタグで)
docker run -it rust-env # コンテナの中に入る
# このレポジトリの内容をコンテナ内の /project にsyncするつつコンテナに入る
docker run -itv /Users/akira/code/rust/docker_rust/epoll_server/:/project rust-env
```

# In Container

```bash
cd project
# run http server
cargo run & # ビルド & バックグラウンドで実行
curl http://127.0.0.1:8080
```
