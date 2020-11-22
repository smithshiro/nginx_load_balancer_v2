# nginx load balancer sample

ロードバランス構成の検証用

## Getting Started

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

origin1_nginx,origin2_nginx,origin3_nginxのどれかにアクセスされているはず
