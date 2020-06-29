# 批量删除提现账号

#### 接口描述：
- 批量删除提现账号。

#### 请求 URL：
- `http|https://host/api/v1/withdraw_user/method/del.withdraw.user.list/`

#### 请求方式：
- GET
- POST

#### 是否授权：
- 需要授权

#### 业务参数：
|参数名|类型|是否必须|范围值|默认值|示例值|描述|
|:----|:---|:---:|:-----|:-----|:-----|-----|
|withdraw_user_id |integer |是 |gt[]:0 | |[3,4] |提现账号编号 |
|client_id |integer |是 |gt:0 | |1 |账号编号 |

#### 响应参数：
|参数名|类型|是否返回|示例值|描述|
|:-----|:-----|:---:|:-----|-----|
|status |integer |是 |200 |状态码 |
|message |string |是 |success |消息信息 |
|data |boolean |是 |true |返回 true 表示执行成功 |

#### 响应示例：
```json
{
  "status": 200,
  "message": "success",
  "data": true
}
```

#### 备注:
无