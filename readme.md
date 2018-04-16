# 在 Laravel 应用中使用 pjax 进行页面加速

> 文章地址：https://curder.com/posts/using-pjax-for-page-acceleration-in-the-laravel-app

## 安装

### 环境文件

在项目的根目录中附带一个`.env.example`文件，请将其拷贝重命名为`.env`。可以使用如下命令完成操作`cp .env.example .env`。

> 注意：确保您的系统上显示隐藏的文件。


### Composer

laravel项目依赖通过[composer](http://getcomposer.org/)工具进行管理。

第一步是通过在终端中进入到项目中并输入以下命令来安装依赖

```php
composer install
```


### artisan命令

我们要做的第一件事就是设置 Laravel 在进行加密时使用的密钥。


```php
php artisan key:generate
```

应该看到一条绿色消息，指出您的密钥已成功生成，以及你应该看到`.env`文件中的`app_key`变量反映出来。

```
php artisan serv
```

使用上面的命令开启一个服务器，现在打开浏览器访问地址: http://127.0.0.1:8000，点击导航栏的**Login**或者**Register**按钮体验 Pjax 和 NProgress ，带来的更好的访问体验。


> 这是一个相对比较简答的项目示例，没有使用到数据库。
