# 第三单元、数据库系统的用户接口以及SQL语言
## DBMS的用户接口

![](https://cdn.jsdelivr.net/gh/ouy0328/database_note/img/20230215134517.png)

- 一个数据库管理系统必须提供一些接口，让用户通过访问这些接口来使用数据库
  - 查询语言（核心），允许用户使用查询语言来访问数据库
    - 形式化查询语言 (SQL 语言)
    - 表格式查询语言
    - 图形化查询语言
    - 受限的自然语言查询 (NITDB)
  - 访问数据库的图形化工具 (GUI)
  - API
  - 类库

#### TQL和GQL的案例

![](https://cdn.jsdelivr.net/gh/ouy0328/database_note/img/20230215142737.png)

### 关系查询语言

![](https://cdn.jsdelivr.net/gh/ouy0328/database_note/img/20230215143553.png)

- 查询语言：让用户有效的从数据库中检索所需的数据。
- 关系模型支持简单，有力的查询语言
  - 有很强的基于逻辑的形式化的基础
  - 实现了有效的查询优化
- 查询语言不是程序设计语言
  - 查询语言不是图灵完备的，不具备逻辑编程能力
  - 查询语言不支持做复杂计算
  - 目的是为了实现简单有效的对大规模数据集进行查询

#### 形式化基础

![](https://cdn.jsdelivr.net/gh/ouy0328/database_note/img/20230215145717.png)

数学化的查询语言

- 关系代数
- 关系演算

SQL语言就是在关系代数和关系演算的基础之上开发出来的语言

ddl数据描述语言, dcl数据控制语言, dml数据操纵语言, ql查询语言

## 15. SQL简介

### SQL语言按照功能可以分为四个子语言

- 数据定义语言 (DDL)，用于定义、删除或修改数据模式
- 查询语言 (QL)，select语句以及select语句中所用到的各种子句，用于数据检索
- 数据操纵语言 (DML)，用于插入、删除或更新数据，对数据库中已经存储的数据进行插、删、改等操作
- 数据控制语言 (DCL)，用于控制用户对数据的访问权限，包括授权、创建用户、审计、语义完整性约束等等

#### 重要术语和概念

- Base table 

  - 基表
  - 关系模型中的关系，在磁盘上存在的

- View 视图

  - 虚表
  - 通过映射或计算得出

- Data type supported
  - 支持的数据类型

- NULL

  - 空值，保留字

- UNIQUE

  - 表示表中的某个属性是否允许有重复值，保留字

- DEFAULT

  - 为数据库中某个表的某个属性指定缺省值，保留字

- PRIMARY KEY 
  - 主键，保留字

- FOREIGN KEY
  - 外键，保留字

- CHECK(Integration Constraint)
  - 为表中的数据定义完整性约束，保留字

## 16. 查询语句基本结构

![](https://cdn.jsdelivr.net/gh/ouy0328/database_note/img/20230209150704.png)

## 17. 简单查询语句

## 18. 基于集合操作的查询语句

## 19. 基于嵌套子查询的查询语句

## 20. 除法与聚集函数计算

## 21. 分组聚集函数计算

## 22. 更复杂的分组聚集函数计算

## 23. CAST与CASE表达式

## 24. 标量子查询

## 25. 表表达式与公共表表达式

## 26. 递归子查询一

## 27. 递归子查询二

## 28. 数据操纵语言

## 29. 关于视图

## 30. 嵌入式SQL

## 31. 使用游标处理查询结果

## 32. 动态SQL与存储过程