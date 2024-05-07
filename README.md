# Neo4j 数据库

这个仓库用于存储与黄河文化项目相关的Neo4j数据库数据，包括节点（Node）和关系（Relation）的定义和数据。

## 项目介绍

此仓库的主要目的是为黄河文化项目提供一个中央存储位置，用于保存和版本控制Neo4j图数据库中的所有节点和关系数据。这些数据可以用于数据恢复、数据迁移、或作为数据分析的基础。

## 数据结构

### 节点（Nodes）
节点数据包含各种实体，如人物、地点、事件等，每个节点的属性根据其类别而有所不同。

### 关系（Relationships）
关系数据定义了节点之间的连接，如“属于”、“位于”或“参与”等。

## 文件结构

- `/nodes` - 存放所有节点数据的文件。
- `/relations` - 存放所有关系数据的文件。

## 使用指南

要使用这些数据，你可以根据需要将其导入到Neo4j数据库中。导入步骤如下：

1. 确保你的Neo4j数据库实例正在运行。
2. 使用Cypher命令或通过Neo4j客户端导入数据。

例如，导入节点数据：

```bash
neo4j-admin import --nodes=nodes/nodes.csv
```

导入关系数据：

```bash
neo4j-admin import --relationships=relations/relationships.csv
```

