# groupchat

#### 介绍
群聊弹幕系统后端。其中netty主要转发广播消息，sprngboot server来存储前端发来的消息。

#### 软件架构
vue-cli3 + springboot + netty


#### 安装教程

1.  将数据库导入主目录下的groupchat.sql（构建数据库和表）
2.  导入idea启动项目

#### 使用说明

1.  根据个人情况修改application.yml里的配置：
端口和路径：
```yml
server:
  port: 7084      #springboot端口
  servlet:
    context-path: /groupchat  #springboot访问路径

netty:
  port: 7000    #netty端口
  context-path: /groupchat   #netty访问路径（和前端保持一致）
```
数据库：
```yml
#   数据源基本配置
  datasource:
    username: root
    password: root
    url: jdbc:mysql://localhost:3306/groupchat?characterEncoding=UTF-8&useSSL=false
    driver-class-name: com.mysql.jdbc.Driver
```

#### 参与贡献

1.  皆非

