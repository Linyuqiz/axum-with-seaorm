# Axum 使用 SeaORM

## Docker 容器配置

```shell
docker run -d --name axemc-postgresql -p 5432:5432  -e POSTGRES_PASSWORD=axemc postgres:latest
docker exec -it axemc-postgresql psql -U postgres -d postgres
```

### 注意点：
- 需要使用 rust stable 版本编译， 否则会报错
- 需要自行启动 postgresql 服务作为数据库
