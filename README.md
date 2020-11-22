# nginx load balancer sample

ロードバランス(キャッシュサーバとオリジンサーバ)構成の検証用

## Getting Started

## Image
![Screenshot from 2020-11-22 17-15-32](https://user-images.githubusercontent.com/27280734/99898643-64318800-2ce6-11eb-8c87-974a8a3b03be.png)
### Prerequisites

docker version
```
$ docker -v
Docker version 19.03.12, build 48a66213fe
```
docker-compose version
```
$ docker-compose -v
docker-compose version 1.26.2, build eefe0d31
```
### Installing

インストール
```
$ docker-compose up -d
```
## Running the tests
http://localhost:10088にアクセス

キャッシュがヒットすればcache1_nginx,cache2_nginx,cache3_nginxが返し
キャッシュが存在しなければorigin1_nginx,origin2_nginx,origin3_nginxにアクセスして返すようになってる
