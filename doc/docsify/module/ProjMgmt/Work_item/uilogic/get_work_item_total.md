## 获取工作项总条数 <!-- {docsify-ignore-all} -->

   

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
state "开始" as Begin <<start>> [[$./get_work_item_total#begin {开始}]]
state "设置总条数" as RAWJSCODE1  [[$./get_work_item_total#rawjscode1 {设置总条数}]]
state "结束" as END1 <<end>> [[$./get_work_item_total#end1 {结束}]]


Begin --> RAWJSCODE1
RAWJSCODE1 --> END1


@enduml
```


### 处理步骤说明

#### 开始 :id=Begin




#### 设置总条数 :id=RAWJSCODE1



<p class="panel-title"><b>执行代码</b></p>

```javascript
const total = uiLogic.ctrl.state.total;
uiLogic.view.layoutPanel.state.data.total = total;
if(!total){
    view.layoutPanel.panelItems.grid.state.visible = false
}else{
    view.layoutPanel.panelItems.grid.state.visible = true
}

```

#### 结束 :id=END1






### 实体逻辑参数

|    中文名   |    代码名    |  数据类型      |备注 |
| --------| --------| --------  | --------   |
|当前视图对象|VIEW|当前视图对象||
|当前部件对象|CTRL|当前部件对象||
|传入变量(<i class="fa fa-check"/></i>)|Default|数据对象||
