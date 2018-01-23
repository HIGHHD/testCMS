+++
title = "Caddy系统"
description = ""

tags = ["应用系统","itop"]

[menu.main]
parent = "applianceSystem"
identifier = "caddy"
weight = 20
+++

### 版本变更记录

|时间|版本|说明|修改人|审核人|
|----|----|----|------|------|
|2018-01-17|V1.0|文档创建|董欣|------|

### 1、 系统概述
#### 1.1 系统背景

#### 1.2 干系人
|序号|公司/部门|角色|联系人|电话|电子邮件|
|----|---------|----|------|----|--------|
|1   |信息技术部|运维工程师|董欣|59366121|dongxin@sczq.com.cn|
|2   |信息技术部|运维工程师|李金闪|59366289|                    |

### 2、 系统环境
#### 2.1 体系结构
![](../images/Caddy系统/Caddy系统.png)

#### 2.2 系统列表
{{%systemInfoData systemName="Caddy系统"  environment="生产环境" /%}}

### 3、 系统监控
通过访问http://http://192.168.1.168:3000/dashboard/db/caddyxi-tong 登录监控系统
1. 虚拟机监控
![](../images/Caddy系统/Caddy系统1.png)
2. Docker主机监控
![](../images/Caddy系统/Caddy系统2.png)



