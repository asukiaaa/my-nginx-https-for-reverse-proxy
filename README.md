# my-nginx-https-for-reverse-proxy

https://localhost へのリクエストを9002に、
https://locaohost/graphql へのリクエストを3000に
仲介します。

## Requirements

- docker
- docker-compose
- mkcert

## Setup

### nginx.confの設定
nginx.confのproxy_pass2箇所のurlを、自身のPCのurlに変更してください。

### mkcertの設定

初期化してください

```
mkcert --init
```


## run

```
docker-compose up
```
