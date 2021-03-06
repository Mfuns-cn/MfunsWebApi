### 修改用户名

### 地址

```url
/module/update/nickname.php
```

### 要求
- 用户已登录
- 非黑名单用户

### 方法
- POST


### 参数

| 参数      | 类型   | 值  | 备注                                                 |
| --------- | ------ | --- | ---------------------------------------------------- |
| nickname  | 字符串 |     | 用户名                                               |
| author_id | 整数   |     | 要更换名字的用户（仅管理员可用，普通用户为自己的id） |

### 返回

| 参数     | 类型   | 值                  | 备注           |
| -------- | ------ | ------------------- | -------------- |
| code     | 整数   | `0`(失败),`1`(成功) | 请求的状态     |
| msg      | 字符串 |                     | 状态的具体说明 |
| nickname | 字符串 |                     | 修改的用户名   |
| self     | 整数   | `0`,`1`             | 是否为自己     |

```json
{
    "code": 1,
    "msg": "修改成功！",
    "nickname": "2333",
    "self": 1
}
```