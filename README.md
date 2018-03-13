# 编译打包
* gradle build -Denv=local
* gradle version 4.6

## MySQL
### 本地配置
* 默认端口3306 
* schema lihe
* 用户  密码 

## 项目module描述
### common
* 公共模块
* 不依赖其他项目module

### lihe-server
* lihe 应用服务器
* 包含server系统功能的代码
* 依赖
* flyway关闭，启动server报错时请在server目录下执行
```
gradle  flywayMigrate -Dport=3307
```
或
```
gradle  flywayMigrate
```