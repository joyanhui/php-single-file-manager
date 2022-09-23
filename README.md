# php单文件管理器

#### 介绍
基于tinyfilemanager  二次开发，修改了部分境内无法访问的cdn，所有修改点都保留了原始代码在注释里面

#### 软件架构
基于 12 Feb 2022 tinyfilemanager-2.4.7，主要修改调用的js和css等文件境内无法访问或者速度超慢的问题。

#### 安装教程

1.  下载
https://gitee.com/joyanhui/php-single-file-manager/repository/archive/master.zip
2.  解压 把 文件上传到服务器，http://youwebsite.com
3.  访问： http://youwebsite.com/_tinyfilemanager.php 即可开始使用

#### 用户名密码

1.  默认用户名 admin  密码：J7*i9WUyFr
2.  修改密码 打开文件搜 $auth_users = array(  修改
3.  获取hash密码 https://tinyfilemanager.github.io/docs/pwd.html
4.  用户user 只有只读权限，默认也删除禁用了，如要使用自行添加

#### 进阶
##### 自定义cdn
把_cdn目录上传到自己的网站，然后替换  _tinyfilemanager.php 里面的 ./_cdn 为你的私有地址即可。
推荐阿里oss 腾讯 cos 以及 ucloud等
##### 外部调用
自行研究吧