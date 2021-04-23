<!--
 * @Author: ChenDoXiu
 * @Description: 
 * @Date: 2021-04-23 22:23:18
 * @LastEditors: ChenDoXiu
 * @LastEditTime: 2021-04-23 22:23:51
 * @FilePath: \MfunsWebApi\content\LikePost.md
-->
## Like 文章

给文章添加一个 like，如果用户已经 like，再次调用为取消
like

### 地址
```
/module/action/like-post.php
```
### 要求
- 用户已登录
- 非黑名单用户

### 方法
- POST

### 参数

| 参数    | 类型 | 值  | 备注     |
| ------- | ---- | --- | -------- |
| post_id | 整数 |     | 文章的id |

### 返回

| 参数 | 类型   | 值    | 备注 |
| ---- | ------ | ----- | ---- |
| code | 整数   | `0`(失败),`1`(成功),`2`(取消) | 请求的状态 |
| msg  | 字符串 |       |   描述 |

```json
{
    "code":"1",
    "msg": "喜欢成功！"
}
```