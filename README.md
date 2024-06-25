# README

## 开发配置

### 数据库创建

```
docker run -d --name db-for-mangosteen -e POSTGRES_USER=mangosteen -e POSTGRES_PASSWORD=123456 -e POSTGRES_DB=mangosteen_dev -e PGDATA=/var/lib/postgresql/data/pgdata -v mangosteen-data:/var/lib/postgresql/data --network=network1 postgres:14
```

## 常见问题

### 测试文档有中文无法进行格式化

> 测试文档首行添加：`# encoding: utf-8`