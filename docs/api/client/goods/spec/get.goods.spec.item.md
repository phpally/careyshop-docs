# 获取一条商品规格

#### 接口描述：
- 获取一条商品规格。

#### 请求 URL：
- `http|https://host/api/v1/spec/method/get.goods.spec.item/`

#### 请求方式：
- GET
- POST

#### 是否授权：
- 否

#### 业务参数：
|参数名|类型|是否必须|范围值|默认值|示例值|描述|
|:----|:---|:---:|:-----|:-----|:-----|-----|
|spec_id |integer |是 |gt:0 | |1 |商品规格编号 |

#### 响应参数：
|参数名|类型|是否返回|示例值|描述|
|:-----|:-----|:---:|:-----|-----|
|status |integer |是 |200 |状态码 |
|message |string |是 |success |消息信息 |
|data |object |否 |[] |返回对象 |

|data|类型|是否返回|示例值|描述|
|:-----|:-----|:---:|:-----|-----|
|spec_id |integer |是 |1 |商品规格编号 |
|goods_type_id |integer |是 |2 |所属商品模型编号 |
|name |string |是 |颜色 |商品规格名称 |
|spec_index |integer |是 |1 |商品规格检索 0=否 1=是 |
|sort |integer |是 |50 |商品规格排序值 |
|spec_item |array |是 |[&#34;黑色&#34;,&#34;红色&#34;] |商品规格项 |

#### 响应示例：
```json
{
  "status": 200,
  "message": "success",
  "data": {
    "spec_id": 1,
    "goods_type_id": 2,
    "name": "颜色",
    "spec_index": 1,
    "sort": 50,
    "spec_item": [
      "黑色",
      "红色"
    ]
  }
}
```

#### 备注:
无