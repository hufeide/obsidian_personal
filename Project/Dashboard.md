---
type: dashboard
updated: 2026-11-04
---

# 工作台

> 这里是入口，不是另一个需要维护的数据库。每天从这里进入，其他内容按链接和查询呈现。

## 当前重点

### 本周最重要的结果
- [x] 完成 Obsidian 知识库上线试点启动，并明确 AI 整理流程试点范围
- [x] 完成首份素材 Ingest（量子位「AI大模型」标签页剪藏录入 Wiki，新建 1 篇 Wiki 文章与账本）
- [x] 编写项目工作流和日报周报生成工作流
- [ ] 完成 Vault 备份

### 当前重点项目
- [[Obsidian知识库上线与AI整理试点]]

### 正在推进的项目
```dataview
TABLE status AS "状态", priority AS "优先级", due AS "截止日期"
FROM "Project"
WHERE type = "project" AND status != "已完成" AND status != "已归档"
SORT priority ASC, due ASC
```

### 最近日志
```dataview
LIST
FROM "03-Areas/日志"
SORT file.name DESC
LIMIT 7
```

### 未完成任务
```tasks
not done
sort by due
limit 20
```

## 每周回顾

- 本周完成了什么？完成知识库上线试点启动；完成首份素材 Ingest（量子位标签页剪藏，1 篇 Wiki 文章、账本和 manifest）；编写项目工作流和日报周报生成工作流。
- 哪件事产生了最大价值？跑通 Wiki 录入闭环（素材 → 来源整理 → 账本 → 索引 → 校验），后续素材可复用同一流程。
- 哪些任务应该停止、推迟或委派？暂停复杂数据库建设；Vault 备份、第 2-3 份资料收集和 AI 整理验证推迟到下周。
- 下周最重要的三个结果是什么？1) 完成 Vault 备份；2) 完成第 2-3 份资料收集和剩余 2 篇资料笔记；3) 完成 1 份录音文稿 AI 整理验证。

---
<small>查询区块需要安装 Dataview 和/或 Tasks 插件；没有插件时可直接使用上方链接与手工清单。</small>
