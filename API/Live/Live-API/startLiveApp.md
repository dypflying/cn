# startLiveApp


## 描述
启用APP

## 请求方式
PUT

## 请求地址
https://live.jdcloud-api.com/v1/apps:start


## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**appName**|String|True| |appName|
|**publishDomain**|String|True| |直播的推流域名|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**requestId**|String|ruquestId|


## 返回码
|返回码|描述|
|---|---|
|**400**|Invalid parameter|
|**401**|Authentication failed|
|**404**|Not found|
|**503**|Service unavailable|
|**200**|OK|
|**500**|Internal server error|
