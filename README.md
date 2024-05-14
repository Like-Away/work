##### 个人信息
- 学号:2111030074
- 姓名:李柯

####  项目访问
- 地址: http://120.76.250.155
        http://120.76.250.155:80
- 普通用户登录:用户名:root         密码:root
- 管理员登录:用户名admin           密码:admin


#### 架构

- 前端：vue全家桶
- 后端： node:express框架
- 数据库：MySQL

#### 基本功能

##### 普通用户

- 注册、登录（图形验证码）
- 定位 （腾讯地图定位功能）、自主选择所在城市
- 商品
  - 分类
  - 简单展示商品
  - 查看商品详情
  - 商品评论
- 分页功能
- 购物车功能
  - 加入购物车
  - 购物车商品数量增减
  - 清空购物车
  - 商品结算
- 多关键词模糊搜索商品 （关键词需为商品名称）
- 用户个人中心
  + 修改用户信息 （头像、昵称、简介...）
  + 修改手机号
  + 修改密码

##### 管理员

- 登录（固定账号密码：admin）
- 查看所有用户
- 查看数据库商品信息
- 商品上架（添加商品）
- 删除/修改商品
- 分页功能



##### 服务器端

- 确认是否全局安装`nodemon`

- `cd web-server`
- `mkdir -p public/uploads`  新建uploads文件夹保存商品图片
- 将`web-server`文件夹下的`webshop.sql`导入`MySQL`数据库中
- `npm install` 安装依赖
- 修改`web-server/src/config.js`文件，此文件记录项目的全局变量，配置文件中的`password`、`database`、`user`属性
- `npm run dev` 在本地运行，启动服务器

##### 客户端

- `cd web-client`
- `mkdir static` 新建static文件夹
- `npm install` 安装依赖
- `npm run dev` 在本地运行
- 接着就可以在`http://localhost:8080`下访问到该项目

