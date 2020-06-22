# TekapoCart_docker_compose

**install mkcert**

```
mkdir docker_compose/ca
cd docker_compose/ca
brew install mkcert
brew install nss
mkcert -install
mkcert tekapocart.devel
```

**modify host file**

```
sudo vim /etc/hosts
127.0.0.1       tekapocart.devel
```

**modify .env**

```
TC_DOMAIN=ToBeDefined
ADMIN_MAIL=ToBeDefined
DB_NAME=tekapocart
DB_USER=tekapocart
DB_PASSWD=ToBeDefined
DB_RT_PASSWD=ToBeDefined
```

**run docker-compose**

```
cd docker_compose
docker-compose up
```

```
curl https://tekapocart.devel:4443
```


