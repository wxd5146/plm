## 日容量(DAY_CAPACITIES) <!-- {docsify-ignore-all} -->

   

### 默认规则 :id=Default

```plantuml
@startuml
hide empty description
<style>
root {
  HyperlinkColor #42b983
}
</style>

state "start" as start  <<start>>
state "end" as end <<end>>
state "默认字符串长度" as a426c150c00257e1ea66687e1c34e024 [[$./Day_capacities#aa426c150c00257e1ea66687e1c34e024 {"默认字符串长度"}]]


start --> a426c150c00257e1ea66687e1c34e024 
a426c150c00257e1ea66687e1c34e024 --> end 


@enduml
```

#### 条件说明

##### 默认字符串长度 :id=aa426c150c00257e1ea66687e1c34e024


*关键条件*


`DAY_CAPACITIES(日容量)` 属性长度在区间 `(0 , 1048576]` 内

> [!ATTENTION|label:规则信息|icon:fa fa-warning]
> 内容长度必须小于等于[1048576]







