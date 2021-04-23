<!--
 * @Author: ChenDoXiu
 * @Description: 
 * @Date: 2021-04-23 23:32:55
 * @LastEditors: ChenDoXiu
 * @LastEditTime: 2021-04-23 23:33:55
 * @FilePath: \MfunsWebApi\content\reward.md
-->
## 打赏

### 地址

```url
/module/action/reward.php
```

### 要求
- 用户已登录
- 非黑名单用户

### 方法
- POST


### 参数

| 参数      | 类型 | 值  | 备注     |
| --------- | ---- | --- | -------- |
| post_id | 整数 |     | 文章id |
|number|整数||金额|
|type|枚举|`post`|未知（但必须要有）|

### 返回值

```json
{
    "code": 1,
    "msg": "打赏成功！",
    "post_url": "https://www.mfuns.cn/1.html"
}
```