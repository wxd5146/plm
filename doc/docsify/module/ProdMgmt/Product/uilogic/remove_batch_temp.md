## 批量删除产品成员临时数据 <!-- {docsify-ignore-all} -->

   

### 处理过程

```plantuml
@startuml
hide footbox
<style>
root {
  HyperlinkColor #42b983
}
</style>

hide empty description
state "开始" as Begin <<start>> [[$./remove_batch_temp#begin {开始}]]
state "批量删除临时数据（临时）" as RAWJSCODE1  [[$./remove_batch_temp#rawjscode1 {批量删除临时数据（临时）}]]
state "结束" as END1 <<end>> [[$./remove_batch_temp#end1 {结束}]]


Begin --> RAWJSCODE1
RAWJSCODE1 --> END1


@enduml
```


### 处理步骤说明

#### 开始 :id=Begin




#### 批量删除临时数据（临时） :id=RAWJSCODE1



<p class="panel-title"><b>执行代码</b></p>

```javascript
return (async function() { 
    // 获取所有临时数据
    const serviceUtil = ibiz.hub.getApp(context.srfappid).deService;
    const service = await serviceUtil.getService(context, 'plmweb.product_member');
    const list = service.local.getList();
    // 遍历临时数据删除
    list.forEach(item => {
        service.local.delete(context, item.id);
    })
    } 
)();

```

#### 结束 :id=END1






### 实体逻辑参数

|    中文名   |    代码名    |  数据类型      |备注 |
| --------| --------| --------  | --------   |
|临时数据列表|list|数据对象列表||
|传入变量(<i class="fa fa-check"/></i>)|Default|数据对象||
