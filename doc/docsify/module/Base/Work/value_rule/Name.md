## 名称(NAME) <!-- {docsify-ignore-all} -->

   

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
state "默认字符串长度" as bdddb90960b745ad2703698dac6f7db5 [[$./Name#abdddb90960b745ad2703698dac6f7db5 {"默认字符串长度"}]]


start --> bdddb90960b745ad2703698dac6f7db5 
bdddb90960b745ad2703698dac6f7db5 --> end 


@enduml
```

#### 条件说明

##### 默认字符串长度 :id=abdddb90960b745ad2703698dac6f7db5


*关键条件*


`NAME(名称)` 属性长度在区间 `(0 , 200]` 内

> [!ATTENTION|label:规则信息|icon:fa fa-warning]
> 内容长度必须小于等于[200]







