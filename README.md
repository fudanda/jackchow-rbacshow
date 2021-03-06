Rbac 演示后台
===============

基于ThinkPHP5.1， layui2.3 的Jackchow/rbac权限包的演示后台

### 安装条件：

 + php版本 >= 5.6.0


### 安装方法：

> Git 安装

使用命令 `git clone https://github.com/jackchow123456/jackchow-rbacshow` 

对了，不要忘了使用 `composer install` 或者 `composer update` 安装对应依赖

> Composer 安装

使用命令 `composer create-project jackchow/rbacshow:dev-master`


## 目录结构

基本主要的目录结构如下：

~~~
www  WEB部署目录（或者子目录）
├─application           应用目录
│  ├─common             公共模块目录（可以更改）
│  ├─admin              后台模块目录
│  │  ├─api             后台模块Api接口目录（放置相应的Api请求文件）
│  │  ├─behavior        表现层目录
│  │  ├─controller      控制器目录
│  │  ├─model           模型目录
│  │  ├─service         服务目录
│  │  ├─view            视图目录
│  │  ├─transformers    Api接口装换器目录 （放置相应的Api转换器文件）
│  │  ├─validate        验证类目录
│  │  └─ ...            更多类库目录
│  │
├─route                 路由定义目录
│  ├─route.php          路由定义
│  ├─api.php            api路由定义
│  └─...                更多
├─extend                扩展类库目录（登录类，接口转换器类）
~~~

## 运行说明

接着上面安装完后 ,并且配置好你到数据库文件。

然后运行命令 `php think migrate:run` 迁移数据文件

然后 `php think seed:run` 填充数据

配置后虚拟主机后 访问 : 该项目虚拟主机名/admin

初始化账号：jack/hurray

初始化密码: 123456

网上demo：http://rbac.pumeiduo.com/admin

## 参与开发
775893055@qq.com

本项目用到`league/fractal`扩展包 用作Api接口数据输出 [了解一下](http://fractal.thephpleague.com/)。

## 版权信息

ThinkPHP遵循Apache2开源协议发布，并提供免费使用。

本项目包含的第三方源码和二进制文件之版权信息另行标注。

版权所有Copyright © 2006-2018 by ThinkPHP (http://thinkphp.cn)

All rights reserved。

ThinkPHP® 商标和著作权所有者为上海顶想信息科技有限公司。

更多细节参阅 [LICENSE.txt](LICENSE.txt)
