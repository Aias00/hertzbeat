---
id: influxdb  
title: 监控：InfluxDB 数据库监控      
sidebar_label: InfluxDB 数据库   
keywords: [开源监控系统, 开源数据库监控, InfluxDB 数据库监控]
---

### 配置参数

|  参数名称  |                        参数帮助描述                        |
|--------|------------------------------------------------------|
| 监控Host | 被监控的对端IPV4，IPV6或域名。注意⚠️不带协议头(eg: https://, http://)。 |
| 任务名称   | 标识此监控的名称，名称需要保证唯一性。                                  |
| 端口     | 数据库对外提供的端口，默认为8086。                                  |
| URL    | 数据库连接URL,一般是由host拼接，不需要添加                            |
| 采集间隔   | 监控周期性采集数据间隔时间，单位秒，可设置的最小间隔为30秒                       |
| 是否探测   | 新增监控前是否先探测检查监控可用性，探测成功才会继续新增修改操作                     |
| 描述备注   | 更多标识和描述此监控的备注信息，用户可以在这里备注信息                          |

### 采集指标

#### 指标集合：influxdb 基本信息

|    指标名称    | 指标单位 | 指标帮助描述 |
|------------|------|--------|
| build_date | 无    | 创建日期   |
| os         | 无    | 操作系统   |
| cpus       | 无    | cpus   |
| version    | 无    | 版本号    |

#### 指标集合：http 响应时间

|     指标名称      | 指标单位 | 指标帮助描述  |
|---------------|------|---------|
| handler       | 无    | handler |
| path          | 无    | 路径      |
| response_code | 无    | 返回code  |
| method        | 无    | 请求方法    |
| user_agent    | 无    | 用户代理    |
| status        | 无    | 状态      |

#### 指标集合：正在排队的 TSM 数

|  指标名称  | 指标单位 | 指标帮助描述 |
|--------|------|--------|
| bucket | 无    | 存储桶    |
| engine | 无    | 引擎类型   |
| id     | 无    | 标识符    |
| level  | 无    | 级别     |
| path   | 无    | 数据文件路径 |

#### 指标集合：HTTP写入请求的字节数量

|   指标名称   | 指标单位 | 指标帮助描述 |
|----------|------|--------|
| endpoint | 无    | 终点     |
| org_id   | 无    | 组织标识符  |
| status   | 无    | 状态     |

#### 指标集合：质量控制请求总数

|  指标名称  | 指标单位 | 指标帮助描述 |
|--------|------|--------|
| result | 无    | 结果     |
| org    | 无    | 组织标识符  |
