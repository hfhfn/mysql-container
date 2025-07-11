# mysql-container
mysql容器，conf和docker-compose配置文件示例

## 项目简介
该项目为MySQL数据库的Docker容器化部署提供配置文件模板及详细说明。适合用于快速搭建本地或测试环境的MySQL服务。

## 文件结构
- [docker-compose.yml](file://D:\AIGC\code\mysql8\docker-compose.yml): Docker Compose 配置文件，用于一键启动MySQL容器。
- `conf.d/`: 存放MySQL配置文件目录。
- `data/`: 数据持久化存储目录。
- `env`文件这里并没有使用，无需关注。

## 使用说明
### 启动容器 
在项目根目录执行以下命令：

```bash
docker compose up -d
```
### 停止容器
```bash
docker compose down
```

## 注意事项
1. 修改`docker-compose.yml`中的环境变量以适应不同场景。
2. 持久化数据建议定期备份，防止意外丢失。
3. 若需定制MySQL配置，请修改`conf.d/`目录下的`my.cnf`文件。

