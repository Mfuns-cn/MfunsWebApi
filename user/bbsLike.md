<!--
 * @Author: ChenDoXiu
 * @Description: 
 * @Date: 2021-04-23 22:59:01
 * @LastEditors: ChenDoXiu
 * @LastEditTime: 2021-04-23 22:59:02
 * @FilePath: \MfunsWebApi\content\bbsLike.md
-->
## 关注圈子

关注圈子，再次调用为取消关注

### 地址

```
/module/action/bbs-like.php
```

### 要求
- 用户已登录
- 非黑名单用户

### 方法
- POST


### 参数

| 参数      | 类型 | 值  | 备注     |
| --------- | ---- | --- | -------- |
| bbs_id | 整数 |     | 圈子id |

### 返回

| 参数 | 类型   | 值    | 备注 |
| ---- | ------ | ----- | ---- |
| code | 整数   | `0`(失败或无权限),`1`(成功),`2`(取消) | 状态码 |
| msg  | 字符串 |       |   状态的具体说明 |

```json
{
    "code":"1",
    "msg": "关注成功！"
}
```
