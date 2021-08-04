# 青龙面板与ninja扫码登录结合

使用

```bash
mkdir -p /data/qinglong-ninja
cd /data/qinglong-ninja
wget https://ghproxy.com/https://raw.githubusercontent.com/gcdd1993/qinglong-ninja/main/docker/docker-compose.yml
docker-compose up -d
```

可以自行修改`docker-compose.yml`中的映射路径
```yaml
volumes:
    - ./config:/ql/config
    - ./log:/ql/log
    - ./db:/ql/db
    - ./repo:/ql/repo
    - ./raw:/ql/raw
    - ./scripts:/ql/scripts
    - ./jbot:/ql/jbot
```