# TekapoCart_docker_compose

**install mkcert**

```
mkdir docker_compose/ca
cd docker_compose/ca
brew install mkcert
brew install nss
mkcert -install
mkcert tekapocart.dev
```

**modify host file**

```
sudo vim /etc/hosts
127.0.0.1       tekapocart.dev
```

**run docker-compose**

```
cd docker_compose
docker-compose up
```

```
curl https://tekapocart.dev:4443
```


