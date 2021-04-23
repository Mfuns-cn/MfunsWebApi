<!--
 * @Author: ChenDoXiu
 * @Description: 
 * @Date: 2021-04-23 23:03:30
 * @LastEditors: ChenDoXiu
 * @LastEditTime: 2021-04-23 23:03:31
 * @FilePath: \MfunsWebApi\content\answer.md
-->

## 问答相关
本api包含 **追加悬赏**，**采纳答案**

### 地址

```
/module/action/answer.php
```


### 要求
- 用户已登录
- 非黑名单用户

### 方法
- POST

### 参数

| 参数      | 类型 | 值  | 备注     |
| --------- | ---- | --- | -------- |
| type | 枚举 |必须， `add`(追加悬赏),`adopt`(采纳答案)    | 操作类型 |
|post_id|整数|必须|文章id|
|number|整数|可选|增加悬赏的金额，仅在追加悬赏时有效|
|comment_id| 整数|可选|采纳的评论id，仅采纳答案时有效|

### 返回

| 参数 | 类型   | 值    | 备注 |
| ---- | ------ | ----- | ---- |
| code | 整数   | `0`(失败或无权限),`1`(成功),`3`(以被采纳) | 状态码 |
| msg  | 字符串 |       |   状态的具体说明 |

```json
{
    "code":"1",
    "msg": "采纳成功！"
}
```