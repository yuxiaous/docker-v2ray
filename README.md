# docker-v2ray
A docker-compose deployment for `v2ray + WebSocket + TLS` setup.

Recommended server: [bandwagonhost.com](https://bandwagonhost.com/aff.php?aff=39559&gid=1)

## 1. CentOS Setup

1. Install tools `yum install -y iperf3 vim git`
2. `./setup-centos7.sh` which does the following

## 2. Ubuntu Setup

1. Install tools `apt-get install -y vim git`
2. `./setup-ubuntu16.sh` which does the following

## 3. Config

Update `./configs/v2ray/config.json`

- `<uuid>`
- `<password>` if necessary
- `<secret>` if necessary

Update `./configs/Caddyfile`

- Replace `localhost:8080` with real domain

## 4. Start

```
docker-compose up
```

Or run as daemon

```
docker-compose up -d
```
