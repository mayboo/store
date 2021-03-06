一款基于php语言开发的服务端API
=====================

[![License](https://poser.pugx.org/topthink/think/license)](https://packagist.org/packages/topthink/think)
####  项目特色
主要基于ThinkPHP5框架基础上,对已有的模式做了更深的强化，优化核心，减少依赖，基于全新的架构思想和命名空间实现，> ThinkPHP5。
详细开发文档参考 [ThinkPHP5完全开发手册](http://www.kancloud.cn/manual/thinkphp5)
项目尤其注重AOP思想、面向对象的高度抽象、RESTFUL的灵活运用,对相应的层可直接复用。
####  验证器的封装

####  异常类的封装

####  TOKEN令牌的获取封装




#### 运行环境
本地环境开发,采用phpStrom开发软件,对应的测试小程序见本库[shops];
## 目录结构
##### 路由配置范例
Route::get('api/:version/banner/:id','api/:version.Banner/getBanner');
Route::get('api/:version/theme','api/:version.Theme/getSimpleList');
Route::get('api/:version/theme/:id','api/:version.Theme/getComplexOne');

Route::get('api/:version/product/recent','api/:version.Product/getRecent');

## 函数和命名类、属性、命名规范

`ThinkPHP5`遵循PSR-2命名规范和PSR-4自动加载规范，并且注意如下规范：
###
*   驼峰和小写
*   类库、函数文件统一以`.php`为后缀；
*   类的文件名均以命名空间定义，并且命名空间的路径和类库文件所在路径一致；
*   类名和类文件名保持一致，统一采用驼峰法命名（首字母大写）；
### 
*   类的命名采用驼峰法，并且首字母大写，例如 `User`、`UserType`，默认不需要添加后缀，例如`UserController`直接命名为`User`；
*   函数的命名使用小写字母和下划线（小写字母开头）的方式，例如 `get_client_ip`；
*   方法的命名使用驼峰法，并且首字母小写，例如 `getUserName`；
*   属性的命名使用驼峰法，并且首字母小写，例如 `tableName`、`instance`；
*   以双下划线“__”打头的函数或方法作为魔法方法，例如 `__call` 和 `__autoload`；


### 数据表和字段
*   数据表和字段采用小写加下划线方式命名，并注意字段名不要以下划线开头，例如 `think_user` 表和 `user_name`字段，不建议使用驼峰和中文作为数据表字段命名。


