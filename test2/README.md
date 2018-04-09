# 实验2：图书管理系统用例建模
|:----------:|:-----:|:--------:|
|201510414113|15软件1班|江自杰|

### 1. 图书管理系统的用例关系图
##### 1.1 用例图PlantUML源码如下
```
@startuml
left to right direction
actor 借书者
actor 游客
actor 图书管理员
actor 系统管理员
rectangle {
    借书者 --> (借阅图书)
    游客 --> (查询图书)
    借书者 --> (归还图书)
    借书者 --> (预订图书)
    借书者 --> (取消预订)
    游客<|-借书者
    图书管理员-->(借出图书)
    图书管理员-->(维护书目):增、删、查、改
    图书管理员-->(维护借书者信息)
    借书者<|-图书管理员
    系统管理员-->(维护图书管理员信息)
    图书管理员<|-系统管理员
}
@enduml
```
##### 1.2. 用例图如下：

![](./Book.png '描述')