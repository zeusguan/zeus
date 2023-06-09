# 基于Vue+Springboot日志监控系统[2023]
## TODO
- [ ] 实现日志在线存储，支持MongoDB and Elastic Search
  - [x] 消息存储到MongoDB
  - [x] 消息存储到ES
- [ ] 支持日志快速搜索，方便定位问题
- [ ] 支持Error日志异常告警，支持通知企业微信，钉钉等

## 使用方法

### 环境

| 中间件     | 版本信息 |
| :--: | ------ |
| ElasticSearch | 7.17.3 |
| MongoDB | 6.0 |

### 存储策略配置
已支持策略：

| 配置项 | 策略              |
| ------ | ----------------- |
| es     | ElasticSearch存储 |
| mongo  | MongoDB存储       |

配置语法：
> 注意：需要在application.yml文件中配置

```yaml
storage:
  strategy:
    type: mongo
```

## 参考资料

1. [MongoDB文档](https://www.mongodb.com/docs/manual/tutorial/getting-started/)
2. [Spring Data ElasticSearch版本对照信息](https://docs.spring.io/spring-data/elasticsearch/docs/current/reference/html/)
3. [Spring Data MongoDB版本对照信息](https://docs.spring.io/spring-data/mongodb/docs/current/reference/html/#get-started:first-steps:spring)
4. [Spring Data Elasticsearch 官方文档](https://docs.spring.io/spring-data/elasticsearch/docs/current/reference/html/#reference)
5. [Spring Data MongoDB 官方文档](https://docs.spring.io/spring-data/mongodb/docs/current/reference/html/#reference)