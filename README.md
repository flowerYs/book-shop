> 通过express框架实现在线图书商城,数据存储在mongodb数据库中。数据使用从当当网抓取来

项目目录介绍
```
./spider 用于抓取书籍数据存储在本地数据库中
前台展示使用了weui实现
```

[管理后台预览地址](http://express.lixuanqi.com/admin/login.html)

用户名:admin  
密码:admin  

[前台展示地址](http://express.lixuanqi.com/books/types)

#### 20170112需要实现以下功能
1. 前台用户注册
2. 管理后台中可以查看已经注册的用户的信息

```
用户注册需要填写的个人信息如下
1. 手机号,作为登录账号使用(mobile)
2. 密码(pwd)
3. 邮箱(email)
4. 姓名(name)
5. 收件地址(address)
6. 注册时间(reg_time,需要你设计数据结构的时候填写默认值)
用户信息的数据集合为 users
用户管理后台的访问地址为:
	列表	/admin/users/list/1
	新增	/admin/users/add
	修改	/admin/users/edit
用户前台注册页面的访问地址为:
	/reg
前台页面要求使用weui实现手机页面效果
```
#### 20170114
1. 前台部分用户登录判断
2. 用户对书籍信息进行购买的时候需要登录
3. 登录的用户显示个人中心
4. 没有登录的用户显示登录页面,在登录页面可以跳转到注册页面
