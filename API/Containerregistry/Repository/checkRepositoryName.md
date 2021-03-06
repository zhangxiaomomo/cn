# checkRepositoryName


## 描述
查询指定镜像仓库名称是否已经存在以及是否符合命名规范。


## 请求方式
POST

## 请求地址
https://openapi.cr.jdcloud.com/v1/regions/{regionId}/repositories:checkRepositoryName

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**regionId**|String|True| |Region ID|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**registryName**|String|True| |注册表名。|
|**repositoryName**|String|True| |待验证的镜像仓库名。|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**requestId**|String| |
|**result**|Result| |

### Result
|名称|类型|描述|
|---|---|---|
|**code**|Integer|表示用户指定的镜像仓库名是否通过校验， 0 通过 1 名称为空 2 不符合规范 3 重名|
|**reason**|String|code字段非零时，给出详细原因。|

## 返回码
|返回码|描述|
|---|---|
|**400**|Invalid parameter|
|**401**|Authentication failed|
|**404**|Not found|
|**503**|Service unavailable|
|**200**|OK|
|**500**|Internal server error|
