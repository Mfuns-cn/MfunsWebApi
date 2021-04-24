## 签到



### 地址

```url
/module/action/sign.php
```

### 要求
- 用户已登录
- 非黑名单用户

### 方法
- POST


### 参数

| 参数      | 类型 | 值  | 备注     |
| --------- | ---- | --- | -------- |
| sign | 整数 |   1  | 必须 |

### 返回

| 参数 | 类型   | 值    | 备注 |
| ---- | ------ | ----- | ---- |
| code | 整数   | `0`(失败),`1`(成功),`2`(重复)| 请求的状态 |
| msg  | 字符串 |       |   状态的具体说明 |
|sign_c|整数||排名|
|content|HTML字符串||网页显示的内容|
|text| 字符串||文本信息|
|text_mobile|字符串||移动端显示的文本|
```json
{
    "code": 1,
    "content": "<li><i class=\"jinsom-icon jinsom-zhifuchenggong\"></i>签到成功</li><li>累计签到14天</li><fieldset class=\"layui-elem-field\"><legend>获得以下奖励</legend><div class=\"layui-field-box\"><li>宅币 * 600</li><li>经验值 * 2</li></div></fieldset>",
    "msg": "签到成功",
    "sign_c": 14,
    "text": "今日已签到",
    "text_mobile": "已签到",
}
```