<!--
 * @Author: ChenDoXiu
 * @Description: 
 * @Date: 2021-04-23 23:18:03
 * @LastEditors: ChenDoXiu
 * @LastEditTime: 2021-04-23 23:20:05
 * @FilePath: \MfunsWebApi\content\addBlacklist.md
-->
## 拉黑用户

拉黑用户，再次调用为取消拉黑

### 地址

```
/module/action/add-blacklist.php
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
| code | 整数   | `0`(失败),`1`(取消),`2`(成功) | 请求的状态 |
| msg  | 字符串 |       |   状态的具体说明 |

```json
{
    "code":"2",
    "msg": "已经加入黑名单！"
}
```