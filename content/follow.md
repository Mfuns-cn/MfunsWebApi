<!--
 * @Author: ChenDoXiu
 * @Description: 
 * @Date: 2021-04-23 22:47:47
 * @LastEditors: ChenDoXiu
 * @LastEditTime: 2021-04-23 22:47:48
 * @FilePath: \MfunsWebApi\content\follow.md
-->
## 关注用户

关注用户，再次调用为取消关注

### 地址

```
/module/action/follow.php
```

### 要求
- 用户已登录
- 非黑名单用户

### 方法
- POST


### 参数

| 参数      | 类型 | 值  | 备注     |
| --------- | ---- | --- | -------- |
| author_id | 整数 |     | 用户的id |

### 返回

| 参数 | 类型   | 值    | 备注 |
| ---- | ------ | ----- | ---- |
| code | 整数   | `0`(失败),`1`(取关),`2`(成功),`3`(相互关注) | 请求的状态 |
| msg  | 字符串 |       |   状态的具体说明 |

```json
{
    "code":"2",
    "msg": "关注成功！"
}
```