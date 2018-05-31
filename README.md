# 信立泰

    ：cd到项目根目录，一次执行
    ：cp .env.example .env
    ：修改.env文件的配置属性(主要是DB_*字段)
    ：composer install -vvv
    : 在本地新建数据库（数据库名使用.env中设置的数据库名）
    ：php artisan migrate
    ：php artisan db:seed
    ：php artisan key:generate
    
##### 入口文件 public/index.php,部署vhost时服务器指向项目的public目录
    
    
## 目录结构
### App/Http/Controllers
    Admin  管理后台模块
    Auth  登录认证模块
    Wechat  微信端模块
    
### App/Http/Routes
    Api.php  接口路由配置文件
    Web.php  PC端路由配置文件
    Wechat.php  微信端路由
    
### App/Model 
    模型目录，与数据库一对一关系
    
### App/Services
    一般用来写每个模块的公用逻辑代码
    
### Resource/views
    admin  管理后台页面都在这里
    wechat  微信端页面都在这里