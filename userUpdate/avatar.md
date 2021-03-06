### 上传Base64格式头像

### 地址

```url
/module/upload/avatar-base64.php
```

### 要求
- 用户已登录
- 非黑名单用户

### 方法
- POST


### 参数

| 参数      | 类型   | 值  | 备注                                                 |
| --------- | ------ | --- | ---------------------------------------------------- |
| base64    | 字符串 |     | 头像的base64                                         |
| author_id | 整数   |     | 要更换头像的用户（仅管理员可用，普通用户为自己的id） |

### 返回

| 参数    | 类型   | 值                  | 备注           |
| ------- | ------ | ------------------- | -------------- |
| code    | 整数   | `0`(失败),`1`(成功) | 请求的状态     |
| msg     | 字符串 |                     | 状态的具体说明 |
| fileurl | 字符串 |                     | 回调的图片直链 |
| self    | 整数   | `0`,`1`             | 是否为自己     |
| name    | 未知   |                     | 未知           |

```json
{
    "code": 1,
    "msg": "上传成功！",
    "file_url": "http://mliii.vqyt.cn/user_files/4444/avatar/95038473_1619232137.jpeg",
    "name": null,
    "self": 1
```