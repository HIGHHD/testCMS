---
date: 2017-06-09T14:31:28+08:00
description: ""
menu:
  main:
    identifier: "OTC"
    parent: applianceSystem
    weight: 20
tags:
- 应用系统
- itop
title: "OTC系统"
---
 <style type="text/css">
table th {
    background: rgba(0,85,160,0.4); 
    font-size: 15px;
    white-space: nowrap; /*表头内容强制在一行显示*/
    text-align:center;
}
table tbody tr:nth-child(2n) {
    background: rgba(158,188,226,0.12); 
}
table tr:hover {
    background: #efefef; 
}
table tr{
    font-size:15px;
    text-align:center;
}

table td:nth-child(1){
    width:120px;
}
 table td:nth-child(2){
    width:80px;
}
table td:nth-child(3){
    width:220px;
}
table td:nth-child(4){
    width:120px;
}
table td:nth-child(5){
    width:60px;
}
table td:nth-child(6){
    width:80px;
}
</style>
# 搞定OTC系统运维#
【版本：V1.0】
首创证券有限责任公司
2017年8月
### 版本信息
<table>
   <tr>
      <td>文件编号</td>  
      <td>文件名称</td>
      <td>版本</td>
      <td>撰写人</td>
      <td>审核人</td>     
   </tr>
   <tr>
      <td>SCZQ-IT-OTC系统-E001</td>
      <td>搞定OTC系统运维</td>  
      <td>V1.0</td>
      <td>纪晓瀛</td>
      <td>纪晓瀛</td>
   </tr>
</table>
### 版本变更记录
<table>
   <tr>
      <td>时间</td>
      <td>版本</td>
      <td>说明</td>
      <td>修改人</td>
      <td>审核人</td>
   </tr>
   <tr>
      <td>2017-08-11</td>
      <td>V1.0</td>
      <td>文档创建</td>
      <td>纪晓瀛</td>
      <td>纪晓瀛</td>
   </tr>
</table>
## 1.	系统概述
### 1.1 	项目背景  
<P style="text-indent:2em;">2012年初证券期货监管工作会议上，证监会主席郭树清表示，以柜台交易为基础，加快建立统一监管的场外交易市场。会议的草案提出，允许证券公司开展柜台交易业务，并对证券公司参与柜台业务的初步条件进行了明确。随后，2012年8月证监会发布了《关于推进证券公司改革开放、创新发展的思路与措施》，再次特别提出要拓展证券公司基础功能，发展证券公司柜台业务。明确指出培育证券公司柜台交易业务，允许证券公司探索面向自己客户的柜台交易市场，将个性化产品通过柜台市场销售给合格投资者，将监管部门或授权机构备案的产品在柜台市场进行转让流通。
<P style="text-indent:2em;">证券公司在此背景下，积极探索建设柜台市场，力图公司内部的交易平台，为投资者提供更加丰富的金融产品和服务，推动证券公司各项业进一步发展、促经营模式转变，以提升证券公司的核心竞争力。
<P style="text-indent:2em;">顶点公司在区域股权市场、金融资产交易所、券商柜台市场等各类私募产品市场有多年建设经验，自2003年开展股权产权交易系统的开发以来，实施了30余家私募股权、债券、金融资产、各类衍生品、现货交易的成功案例。是目前案例最为丰富、系统最为成熟的供应商。
### 1.2	项目干系人	

<table>
   <tr>
      <td>序号</td>
      <td>部门</td>
      <td>角色</td>
      <td>负责内容</td>
      <td>联系人</td>
      <td>电话</td>
      <td>电子邮件</td>
   </tr>
   <tr>
      <td>1</td>
      <td>经纪业务部、各地营业部</td>
      <td>最终用户</td>
      <td>业务运营</td>
      <td>张蕴璞、魏显翠</td>
      <td>010-59366245、010-59366048</td>
      <td></td>
   </tr>
   <tr>
      <td>2</td>
      <td>清算部</td>
      <td>最终用户</td>
      <td>系统清算</td>
      <td>艾旭军、王渺</td>
      <td>010-59323911、010-59366236</td>
      <td></td>
   </tr>
   <tr>
      <td>3</td>
      <td>信息技术部</td>
      <td>系统管理员</td>
      <td>系统维护</td>
      <td>纪晓瀛、方国聪</td>
      <td>010-59323908</td>
      <td></td>
   </tr>
   <tr>
      <td>4</td>
      <td>合规部</td>
      <td>权限管理员</td>
      <td>审核权限</td>
      <td>康玲</td>
      <td>010-59366080</td>
      <td></td>
   </tr>
   <tr>
      <td>5</td>
      <td>顶点公司</td>
      <td>开发商</td>
      <td>技术支持</td>
      <td>顶点</td>
      <td>0591-87861000转6、0591-87866888转301-307</td>
      <td></td>
   </tr>
   <tr>
      <td>6</td>
      <td>资金运营管理部</td>
      <td>最终用户</td>
      <td>产品挂牌</td>
      <td>李佳欢</td>
      <td>010-59366214</td>
      <td></td>
   </tr>
   <tr>
      <td>7</td>
      <td>中证资本</td>
      <td>交易所</td>
      <td>技术支持</td>
      <td>客服</td>
      <td>010-83897913，83897869</td>
      <td></td>
   </tr>
   <tr>
      <td>8</td>
      <td>电信、联通</td>
      <td>运营商</td>
      <td>通信线路</td>
      <td>集团客服</td>
      <td>10000、10010</td>
      <td></td>
   </tr>
</table>
### 1.3技术路线
<P style="text-indent:2em;">OTC系统使用oracle 10g数据库，采用C++语言作为中间件开发语言， 通过DLL动态链接库提供中间件的基础服务，同时采用Java语言作为中间件应用监控程序开发语言， 通过应用监控平台监控各个中间件服务的运行状态；Web应用采用Java语言作为应用开发语言。
## 2.	系统环境  
### 2.1	整体体系结构
<P style="text-indent:2em;">公司采用全流程模式与中证资本进行系统对接，全流程模式是指私募产品在报价系统发行，公司柜台交易系统发起的业务申请采用实时消息的方式报送到报价系统。公司柜台交易系统与报价系统对接后，使用报价系统提供的发行交易、注册登记和资金交收功能。 
在全流程模式下，参与人可以通过柜台交易系统在报价系统中开展认购、申购、赎回、分红和转让业务。
<P style="text-indent:2em;">公司OTC业务系统由OTC报价系统、集中交易、账户管理、交易终端及法人清算等部分组成，外部通过深证通与市场检测中心进行对接。根据公司现有的系统情况，采用现有集中交易、账户管理、法人清算、交易终端系统升级相关模块同时增加OTC报价系统方案部署。
#### 2.1.1	相关系统列表  
<table>
   <tr>
      <td>序号</td>
      <td>系统</td>
      <td>开发商</td>
      <td>技术部联系人</td>
      <td>备注</td>
   </tr>
   <tr>
      <td>1</td>
      <td>集中交易</td>
      <td>顶点</td>
      <td>技术部运维组</td>
      <td>资金调拨等</td>
   </tr>
   <tr>
      <td>2</td>
      <td>一柜通</td>
      <td>顶点</td>
      <td>李娟娟、张洪旭</td>
      <td>开户、账户管理</td>
   </tr>
   <tr>
      <td>3</td>
      <td>顶点报盘</td>
      <td>顶点</td>
      <td>纪晓瀛、方国聪</td>
      <td>委托通过顶点报盘发送至深证通消息平台</td>
   </tr>
   <tr>
      <td>4</td>
      <td>深证通消息通信网关（BSMR）</td>
      <td>深证通</td>
      <td>张宇昂、林沙沙</td>
      <td>委托通过深证通平台发送到中证资本</td>
   </tr>
   <tr>
      <td>5</td>
      <td>FDEP</td>
      <td>深证通</td>
      <td>张宇昂、林沙沙</td>
      <td>通过深证通文件传输系统接收中正资本发送的行情文件</td>
   </tr>
   <tr>
      <td>6</td>
      <td>风控系统</td>
      <td>恒生</td>
      <td>李娟娟、张洪旭</td>
      <td></td>
   </tr>
   <tr>
      <td>7</td>
      <td>CRM系统</td>
      <td>顶点</td>
      <td>张洪旭、纪晓瀛</td>
      <td>采集资产等信息</td>
   </tr>
   <tr>
      <td>8</td>
      <td>番茄财富</td>
      <td>思迪</td>
      <td>魏显翠</td>
      <td>思迪运维</td>
   </tr>
   <tr>
      <td>9</td>
      <td>网上交易</td>
      <td>通达信</td>
      <td>李永乐、谢灵运</td>
      <td></td>
   </tr>
   <tr>
      <td>10</td>
      <td>清算系统</td>
      <td>顶点、新意</td>
      <td>清算部</td>
      <td></td>
   </tr>
</table>
#### 2.1.2总体架构
![](../images/OTC1.png)
#### 2.1.3	相关系统交互方式 
![](../images/OTC2.png)
![](../images/OTC3.png)
### 2.2	内部体系结构  
#### 2.2.1	子系统列表
<table>
   <tr>
      <td>序号</td>
      <td>子系统</td>
      <td>备注</td>
   </tr>
   <tr>
      <td>1</td>
      <td>MCenter</td>
      <td>向各模块发送消息包</td>
   </tr>
   <tr>
      <td>2</td>
      <td>FOS</td>
      <td>连接数据库实现对业务数据的操作</td>
   </tr>
   <tr>
      <td>3</td>
      <td>BLS</td>
      <td>调用FOS、BLS实现业务功能</td>
   </tr>
   <tr>
      <td>4</td>
      <td>RS</td>
      <td>实现通信数据的路由转发</td>
   </tr>
   <tr>
      <td>5</td>
      <td>数据库</td>
      <td>存储系统及业务数据</td>
   </tr>
   <tr>
      <td>6</td>
      <td>TOMCAT</td>
      <td>提供前端操作界面</td>
   </tr>
   <tr>
      <td>7</td>
      <td>顶点报盘</td>
      <td>将委托表数据打包成消息发送至bsmr</td>
   </tr>
</table>
#### 2.2.2	部署图
![](../images/OTC4.png)
### 2.3	服务器  
#### 2.3.1	生产环境  
##### 2.3.1.1	服务器硬件列表
<table>
   <tr>
      <td>序号</td>
      <td>用途</td>
      <td>KVM端口</td>
      <td>应用列表</td>
      <td>机器序列号</td>
      <td>实机</td>
      <td>虚拟 </td>
      <td>内网IP</td>
      <td>内存(G)</td>
      <td>硬盘</td>
      <td>CPU</td>
      <td>网络接口</td>
   </tr>
   <tr>
      <td>M1</td>
      <td>主用数据库服务器</td>
      <td>[OTC-SERVER-#40]</td>
      <td>ORACLE/九桥同步</td>
      <td></td>
      <td>1</td>
      <td>0</td>
      <td>192.168.18.131</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>M2</td>
      <td>备用数据库服务器</td>
      <td>[OTC-SERVER-#40]</td>
      <td>ORACLE/九桥同步</td>
      <td></td>
      <td>1</td>
      <td>0</td>
      <td>192.168.18.130</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>M3</td>
      <td>主用TOMCAT服务器</td>
      <td>[OTC-SERVER-#40]</td>
      <td>TOMCAT</td>
      <td></td>
      <td>1</td>
      <td>0</td>
      <td>192.168.18.132</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>M4</td>
      <td>备用TOMCAT服务器</td>
      <td>[OTC-SERVER-#40]</td>
      <td>TOMCAT</td>
      <td></td>
      <td>1</td>
      <td>0</td>
      <td>192.168.18.133</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>M5</td>
      <td>主用中间件服务器</td>
      <td>[OTC-SERVER-#40]</td>
      <td>顶点中间件、报盘</td>
      <td></td>
      <td>1</td>
      <td>0</td>
      <td>192.168.18.134</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>M6</td>
      <td>备用中间件服务器</td>
      <td>[OTC-SERVER-#40]</td>
      <td>顶点中间件、报盘</td>
      <td></td>
      <td>1</td>
      <td>0</td>
      <td>192.168.18.135</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
</table>
##### 2.3.1.2	服务器软件列表
<table>
   <tr>
      <td>序号</td>
      <td>用途</td>
      <td>软件</td>
   </tr>
   <tr>
      <td>M1</td>
      <td>主用数据库服务器</td>
      <td>ORACLE、九桥同步</td>
   </tr>
   <tr>
      <td>M2</td>
      <td>备用数据库服务器</td>
      <td>ORACLE、九桥同步</td>
   </tr>
   <tr>
      <td>M3</td>
      <td>主用TOMCAT服务器</td>
      <td>TOMCAT</td>
   </tr>
   <tr>
      <td>M4</td>
      <td>备用TOMCAT服务器</td>
      <td>TOMCAT</td>
   </tr>
   <tr>
      <td>M5</td>
      <td>主用中间件服务器</td>
      <td>ABOSS2、AUTOIT、oracle、RealVNC、Symantec、JAVA</td>
   </tr>
   <tr>
      <td>M6</td>
      <td>备用中间件服务器</td>
      <td>ABOSS2、AUTOIT、oracle、RealVNC、Symantec、JAVA</td>
   </tr>
</table>
##### 2.3.1.3	数据文件
<table>
   <tr>
      <td>序号</td>
      <td>服务器</td>
      <td>文件说明</td>
      <td>文件路径</td>
      <td>文件来源</td>
      <td>更新频率</td>
      <td>备注</td>
   </tr>
   <tr>
      <td>F1</td>
      <td>M4</td>
      <td>中证资本行情文件</td>
      <td>/home/webuser/app/otc/QSFILE/yyyymmdd/FundDay/OFD_ZZ_189_yyyymmdd_07.TXT</td>
      <td>FDEP-中证资本</td>
      <td>一次性文件</td>
      <td></td>
   </tr>
   <tr>
      <td>F2</td>
      <td>M4</td>
      <td>中证资本清算文件</td>
      <td>/home/webuser/app/otc/QSFILE/yyyymmdd/DisFile/OFD_899_189_yyyymmdd_xx.TXT</td>
      <td>FDEP-中证资本</td>
      <td>一次性文件</td>
      <td></td>
   </tr>
</table>
### 2.4	数据库  
####  2.4.1  生产环境
##### 2.4.1.1	数据库实例  
<table>
   <tr>
      <td>序号</td>
      <td>数据库服务器名称</td>
      <td>版本</td>
      <td>IP地址</td>
      <td>端口号</td>
      <td>实例名</td>
      <td>备注</td>
   </tr>
   <tr>
      <td>DB1</td>
      <td>主用数据库服务器</td>
      <td>Oracle 10g</td>
      <td>192.168.18.131</td>
      <td>1521</td>
      <td>OTCDB</td>
      <td></td>
   </tr>
   <tr>
      <td>DB2</td>
      <td>备用数据库服务器</td>
      <td>Oracle 10g</td>
      <td>192.168.18.130</td>
      <td>1521</td>
      <td>OTCDB</td>
      <td></td>
   </tr>
</table>
##### 2.4.1.2	数据库用户及表空间  
<table>
   <tr>
      <td>序号</td>
      <td>表空间</td>
      <td>用户名</td>
      <td>密码</td>
      <td>备注</td>
   </tr>
   <tr>
      <td>DU1</td>
      <td>FPSS</td>
      <td>FPSS</td>
      <td>OTC_FPSS</td>
      <td></td>
   </tr>
   <tr>
      <td>DU2</td>
      <td>LIVEBOS</td>
      <td>LIVEBOS</td>
      <td>OTC_LIVEBOS</td>
      <td></td>
   </tr>
   <tr>
      <td>DU3</td>
      <td>FPSS_HIS</td>
      <td>FPSS_HIS</td>
      <td>OTC_FPSS_HIS</td>
      <td></td>
   </tr>
   <tr>
      <td>DU4</td>
      <td>EIMAGE</td>
      <td>EIMAGE</td>
      <td>OTC_EIMAGE</td>
      <td></td>
   </tr>
   <tr>
      <td>DU5</td>
      <td>FPSS_3RD</td>
      <td>FPSS_3RD</td>
      <td>OTC_FPSS_3RD</td>
      <td></td>
   </tr>
   <tr>
      <td>DU6</td>
      <td>PRODUCT</td>
      <td>PRODUCT</td>
      <td>OTC_PRODUCT</td>
      <td></td>
   </tr>
   <tr>
      <td>DU7</td>
      <td>ADA</td>
      <td>TEMP</td>
      <td>ADA</td>
      <td></td>
   </tr>
</table>
##### 2.4.1.3	常用数据库表说明  
###### 2.4.1.3.1	产品授权（aboss.tcpxlh）
### 2.5	应用程序  
#### 2.5.1	生产环境  
##### 2.5.1.1	应用程序列表  
<table>
   <tr>
      <td>序号</td>
      <td>服务名称</td>
      <td>IP地址</td>
      <td>存放路径</td>
      <td>开放端口</td>
      <td>备注</td>
   </tr>
   <tr>
      <td>1</td>
      <td>ORACLE/九桥同步</td>
      <td>192.168.18.131</td>
      <td></td>
      <td>1521、8303</td>
      <td></td>
   </tr>
   <tr>
      <td>2</td>
      <td>ORACLE/九桥同步</td>
      <td>192.168.18.130</td>
      <td></td>
      <td>1521、8304</td>
      <td></td>
   </tr>
   <tr>
      <td>3</td>
      <td>TOMCAT</td>
      <td>192.168.18.132</td>
      <td></td>
      <td>8020</td>
      <td></td>
   </tr>
   <tr>
      <td>4</td>
      <td>TOMCAT</td>
      <td>192.168.18.133</td>
      <td></td>
      <td>8020</td>
      <td></td>
   </tr>
   <tr>
      <td>5</td>
      <td>MCENTER</td>
      <td>192.168.18.134</td>
      <td></td>
      <td>5001</td>
      <td></td>
   </tr>
   <tr>
      <td>6</td>
      <td>FOS</td>
      <td>192.168.18.134、192.168.18.135</td>
      <td></td>
      <td>7016</td>
      <td></td>
   </tr>
   <tr>
      <td>7</td>
      <td>BLS</td>
      <td>192.168.18.134、192.168.18.135</td>
      <td></td>
      <td>9009</td>
      <td></td>
   </tr>
   <tr>
      <td>8</td>
      <td>RS</td>
      <td>192.168.18.134、192.168.18.135</td>
      <td></td>
      <td>9109</td>
      <td></td>
   </tr>
   <tr>
      <td>9</td>
      <td>OTCTranSZT</td>
      <td>192.168.18.134、192.168.18.135</td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>10</td>
      <td>AxSvrMgr</td>
      <td>192.168.18.134</td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
</table>
### 2.7	客户端  
#### 2.7.1	生产环境  
##### 2.7.1.1	常用菜单  
生产环境严格控制权限，因此本节只有部分菜单介绍  
<table>
   <tr>
      <td>序号</td>
      <td>菜单代码</td>
      <td>菜单名称</td>
      <td>备注</td>
   </tr>
   <tr>
      <td>1</td>
      <td>10004</td>
      <td>员工管理</td>
      <td>新增、删除员工；改变员工状态如正常、冻结等</td>
   </tr>
</table>
### 2.8	网络　　
#### 2.8.1	生产环境  
##### 2.8.1.1	静态路由  
##### 2.8.1.2	访问控制  
  
<table>
   <tr>
      <td>源程序</td>
      <td>目标程序</td>
      <td>序号</td>
      <td>源服务器</td>
      <td>目标服务器IP</td>
      <td>目标端口</td>
   </tr>
   <tr>
      <td>融资融券中间件</td>
      <td>融资融券数据库</td>
      <td>1</td>
      <td>192.168.18.25</td>
      <td>172.3.0.100</td>
      <td>1521</td>
   </tr>
</table>
## 3.	运维流程  
### 3.1	日常流程  
#### 3.1.1	日操作  
##### 3.1.1.1	开市操作  
<table>
   <tr>
      <td>序号</td>
      <td>时间</td>
      <td>KVM/服务器名称</td>
      <td>操作内容</td>
      <td>结果判断</td>
      <td>备注</td>
   </tr>
   <tr>
      <td>1</td>
      <td>无</td>
      <td>【SZV5-43#-01】DDV5-HQZH-54</td>
      <td>1、 关闭行情网关CMD窗口，双击运行桌面行情网关程序</td>
      <td>1、网关启动后，界面出现“ready、process”等提示即成功</td>
      <td>清除缓存，重连交易所网关</td>
   </tr>
</table>
##### 3.1.1.2	盘间监控  
##### 3.1.1.3	闭市操作  
##### 3.1.1.4	收盘 
##### 3.1.1.5	清算 
#### 3.1.2	周操作  
##### 3.1.2.1	清理数据库备份文件  
<P style="text-indent:2em;">检查192.168.18.25的D、E盘backup文件夹中的每日dmp文件是否都在M盘有对应rar文件，有则删除D、E盘n日前（根据空间决定，不必完全删除）的备份文件。  
#### 3.1.3	月操作  
##### 3.1.3.1	重启服务器  
1、	在16:00前，通知经济业务部、清算部、营业部，将对系统进行维护。  
2、	16:00，在【2-5】RZRQ-FOS-25上关闭所有中间件服务。  
3、	按KVM顺序，依次重启下列服务器：  
4、	检查服务器重启情况，如有LOSAP服务未启动，手工启动；  
5、	在【2-5】RZRQ-FOS-25上开启所有中间件服务；  
6、	通知相关部门系统恢复使用。  
#### 3.1.4	季操作  
##### 3.1.4.1	清理未归档文件  
1、	使用plsql查询当前数据库（rzrqrac1）中未归档表的最早日期（select min(wtrq) from securities.tdrwt_wgd），应留存至少x个月的数据，记住该日期。  
2、	运行ADA.exe登录当前数据库，“日常管理”-“数据清理”，选择“起始日期”（程序在这里表述有误，该日期实际为截止日期），点击“全选”，确认后点击“开始清理”。  
#### 3.1.5	年操作  
##### 3.1.5.1	创建交易年历  
### 3.2	非日常流程  
#### 3.2.4	周末测试流程  
##### 3.2.4.1	主切备流程  
<table>
   <tr>
      <td>序号</td>
      <td>时间</td>
      <td>KVM/服务器名称</td>
      <td>操作内容</td>
      <td>结果判断</td>
      <td>备注</td>
   </tr>
   <tr>
      <td>1</td>
      <td>清算后、测试前</td>
      <td>所有服务器</td>
      <td>1、与清算确认后，关闭下列程序<br>交易所、深交所报盘程序及网关；<br>顶点、转融通报盘程序；<br>银行存管程序；<br>Filetrans程序；</td>
      <td>防止程序保持数据库连接</td>
      <td></td>
   </tr>
</table>
## 4.	系统监控  
### 4.1	监控工具  
#### 4.1.1	OpManager
<P style="text-indent:2em;">ManageEngine OpManager软件可对网络，系统以及应用进行全面的监视.它提供完整的故障管理和性能管理功能，通过综合控制台操作者可实现对路由器、交换机、服务器以及打印机等性能的监视。它包含了许多图、报表，可为操作者提供大量的有关网络、服务器和应用的状态的有用信息。  
##### 4.1.1.1	OpManager安装部署  
OpManager部署服务器为：192.168.4.200  
##### 4.1.1.2	OpManager使用简介  
登录方式：浏览器访问：http://192.168.4.200  
## 5.	常见问题及解决方案  
## 6.	参考文档  