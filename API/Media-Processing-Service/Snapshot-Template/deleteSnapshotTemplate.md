# deleteSnapshotTemplate


## 描述
删除截图模板

## 请求方式
DELETE

## 请求地址
https://mps.jdcloud-api.com/v1/snapshotTemplates/{templateId}


## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**templateId**|String|True| |模板ID|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**requestId**|String|请求ID|


## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
|**400**|Invalid parameter|
|**401**|Authentication failed|
|**404**|Not found|
|**500**|Internal server error|
|**503**|Service unavailable|

## 请求示例
DELETE
```
https://mps.jdcloud-api.com/v1/snapshotTemplates/c35a7f843a6e49a4a32b1f8fab99fbd8

```
