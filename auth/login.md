## 用户登录和认证

### cookie 登录

此api会返回一个格式为 `wordpress_logged_in_一个随机sign` 的 Cookie ，客户端应该保存此 cookie 以请求那些需要用户登录的接口


#### 接口

```url
/module/action/like-post.php
```

#### 方法 
- POST

#### 参数

| 参数      | 类型   | 值  | 备注   |
| --------- | ------ | --- | ------ |
| username  | 字符串 |     | 用户名 |
| apassword | 字符串 |     | 密码   |