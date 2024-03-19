## 工作流(PSWFID) <!-- {docsify-ignore-all} -->

   

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
state "默认字符串长度" as 2f1beb3c0e9897b1e717000331646fd2 [[$./PSWFId#a2f1beb3c0e9897b1e717000331646fd2 {"默认字符串长度"}]]


start --> 2f1beb3c0e9897b1e717000331646fd2 
2f1beb3c0e9897b1e717000331646fd2 --> end 


@enduml
```

#### 条件说明

##### 默认字符串长度 :id=a2f1beb3c0e9897b1e717000331646fd2


*关键条件*


`PSWFID(工作流)` 属性长度在区间 `(0 , 100]` 内

> [!ATTENTION|label:规则信息|icon:fa fa-warning]
> 内容长度必须小于等于[100]






