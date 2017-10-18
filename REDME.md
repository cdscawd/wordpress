

# 本机安装 wordpress，从而能在本地建站，折腾并调试。
- 首先按照前文在Mac下安装XAMPP所述，安装XAMPP；
- 为wordpress安装数据库。wordpress自身是不带数据库的，需要我们在XAMPP中创建数据库。在浏览器中输入：http://localhost/phpmyadmin/，进入数据库管理界面。输入数据库名：wordpress（可自定义），数据库格式选择：utf8_general_ci，链接校对选择：utf8_unicode_ci。然后点击创建。
- 下载wordpress(目前为3.3.1版本)，然后解压 wordpress至：/Applications/XAMPP/xamppfiles/htdocs/ 下。
- 修改配置文件。拷贝 /Applications/XAMPP/xamppfiles/htdocs/wordpress/wp-config-sample.php 至 /Applications/XAMPP/xamppfiles/htdocs/wordpress/wp-config.php，然后用记事本打开，进行如下三处修改：修改数据库名称database_name_here为你的数据库名，在本例中是wordpress修改数据库用户名username_here为root修改数据库密码为空，就是把password_here删除
- 在浏览器中输入：http://localhost/wordpress/，你应该可以看到如下设置页面！
- 在这个设置页面设置站点标题，登陆用户名，密码即可。

## 备注：
```
    wp-config.php 为数据库相关配置文件
```
