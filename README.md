# ThinkPHPTest
使用ThinkPHP3.2.3框架快速搭建网站

一、获取ThinkPHP
获取ThinkPHP的方式很多，官方网站（http://thinkphp.cn）是最好的下载和文档获取来源。
官网提供了稳定版本的下载：http://thinkphp.cn/down/framework.html
如果你希望保持最新的更新，可以通过github获取当前最新的版本（完整版）。

Git获取地址列表（你可以选择一个最快的地址）：
Github： https://github.com/liu21st/thinkphp
Oschina： http://git.oschina.net/liu21st/thinkphp.git
Code： https://code.csdn.net/topthink2011/ThinkPHP

二、运行环境要求
PHP版本要求
PHP5.3以上版本（注意：PHP5.3dev版本和PHP6均不支持）

这里我们推荐使用集成开发环境WAMPServer（wampserver是一个集成了Apache、PHP和MySQL的开发套件，而且支持不同PHP版本、MySQL版本和Apache版本的切换）来使用ThinkPHP进行本地开发和测试。

三、ThinkPHP框架结构
    ├─ThinkPHP 框架系统目录（可以部署在非web目录下面）
    │  ├─Common       核心公共函数目录
    │  ├─Conf         核心配置目录 
    │  ├─Lang         核心语言包目录
    │  ├─Library      框架类库目录
    │  │  ├─Think     核心Think类库包目录
    │  │  ├─Behavior  行为类库目录
    │  │  ├─Org       Org类库包目录
    │  │  ├─Vendor    第三方类库目录
    │  │  ├─ ...      更多类库目录
    │  ├─Mode         框架应用模式目录
    │  ├─Tpl          系统模板目录
    │  ├─LICENSE.txt  框架授权协议文件
    │  ├─logo.png     框架LOGO文件
    │  ├─README.txt   框架README文件
    │  └─index.php    框架入口文件

四、入口文件定义
// 定义应用目录
define('APP_PATH','./Apps/');
// 定义运行时目录
define('RUNTIME_PATH','./Runtime/');
// 开启调试模式
define('APP_DEBUG',True);
// 更名框架目录名称，并载入框架入口文件
require './Think/ThinkPHP.php';

这样最终的应用目录结构如下：
www  WEB部署目录（或者子目录）
├─index.php       应用入口文件
├─Apps            应用目录
├─Public          资源文件目录
├─Runtime         运行时目录
└─Think           框架目录

在浏览器里面输入：http://localhost/xxx/index.php

出现欢迎界面，框架搭建成功


更多精彩内容敬请关注微信公众号：IT-ddd
