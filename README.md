# sub-web-clean
自用修改版
### 使用方法：
建议使用Docker一键部署:
```
docker run -d --restart unless-stopped -p 8090:80 --name sub-web-clean rico-chen/sub-web-modify
```
或使用docker compose
```yaml
name: sub-web-clean
services:
    sub-web-clean:
        restart: unless-stopped
        privileged: false
        ports:
            - 8090:80
        container_name: sub-web-clean
        image: rico-chen/sub-web-clean
```
运行docker compose: `docker compose up -d`
