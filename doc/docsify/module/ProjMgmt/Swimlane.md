# 泳道(Swimlane)  <!-- {docsify-ignore-all} -->



## 属性
|    中文名 | 属性名称           | 类型     | 长度     |值规则   |  序列     | 快速搜索     |  备注  |
| --------   |------------| -----  | -----  | ----- | -----  | :---:   |  -------- |
|建立时间|CREATE_TIME|日期时间型|0|||||
|建立人|CREATE_MAN|文本，可指定长度|100|[默认规则](module/ProjMgmt/Swimlane/value_rule/Create_man#default)||||
|更新时间|UPDATE_TIME|日期时间型|0|||||
|名称|NAME|文本，可指定长度|200|[默认规则](module/ProjMgmt/Swimlane/value_rule/Name#default)||√||
|标识|ID|全局唯一标识，文本类型，用户不可见|100|[默认规则](module/ProjMgmt/Swimlane/value_rule/Id#default)||||
|更新人|UPDATE_MAN|文本，可指定长度|100|[默认规则](module/ProjMgmt/Swimlane/value_rule/Update_man#default)||||
|看板标识|BOARD_ID|外键值|100|[默认规则](module/ProjMgmt/Swimlane/value_rule/Board_id#default)||||
|项目标识|PROJECT_ID|外键值|100|[默认规则](module/ProjMgmt/Swimlane/value_rule/Project_id#default)||||


## 关系
<!-- tabs:start -->


#### **主关系**
| 名称     |   从实体 | 关系类型     |   备注  |
| -------- |---------- |------------|----- |
|[DER1N_WORK_ITEM_SWIMLANE_SWIMLANE_ID](der/DER1N_WORK_ITEM_SWIMLANE_SWIMLANE_ID)|[工作项(WORK_ITEM)](module/ProjMgmt/Work_item)|1:N关系||

#### **从关系**
|  名称   | 主实体   | 关系类型   |    备注  |
| -------- |---------- |-----------|----- |
|[DER1N_SWIMLANE_BOARD_BOARD_ID](der/DER1N_SWIMLANE_BOARD_BOARD_ID)|[看板(BOARD)](module/ProjMgmt/Board)|1:N关系||
|[DER1N_SWIMLANE_PROJECT_PROJECT_ID](der/DER1N_SWIMLANE_PROJECT_PROJECT_ID)|[项目(PROJECT)](module/ProjMgmt/Project)|1:N关系||
<!-- tabs:end -->

## 行为
| 中文名    | 代码名    | 类型    | 事务   | 批处理   | 附加操作  | 插件    |  备注  |
| -------- |---------- |----------- |------------|----------|---------| ----- | ----- |
|Create|Create|内置方法|默认|不支持||||
|Update|Update|内置方法|默认|不支持||||
|Remove|Remove|内置方法|默认|支持||||
|Get|Get|内置方法|默认|不支持||||
|GetDraft|GetDraft|内置方法|默认|不支持||||
|CheckKey|CheckKey|内置方法|默认|不支持||||
|Save|Save|内置方法|默认|不支持||||




## 数据查询
| 中文名    | 代码名    | 默认查询 | 是否权限使用 | 自定义SQL |  备注|
| --------  | --------   | :---:  | :---:  | :---:  |----- |
|[数据查询(DEFAULT)](module/ProjMgmt/Swimlane/query/Default)|DEFAULT|是|否 |否 ||
|[默认（全部数据）(VIEW)](module/ProjMgmt/Swimlane/query/View)|VIEW|否|否 |否 ||


## 数据集合
| 中文名  | 代码名  | 类型 | 默认集合 |   插件|   备注|
| --------  | --------   | --------   | :---:   | ----- |----- |
|[数据集(DEFAULT)](module/ProjMgmt/Swimlane/dataset/Default)|DEFAULT|数据查询|是|||




## 搜索模式
|   搜索表达式   |    属性名    |    搜索模式        |
| -------- |------------|------------|
|N_NAME_LIKE|名称|LIKE|
|N_ID_EQ|标识|EQ|
|N_BOARD_ID_EQ|看板标识|EQ|
|N_PROJECT_ID_EQ|项目标识|EQ|




