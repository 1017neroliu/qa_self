# 后端与 Agent 开发知识库

用场景题检验自己的理解，记录答对了什么、哪里需要修正，以及哪些结论依赖具体前提。

| 分类 | 笔记 | 复习重点 |
| --- | --- | --- |
| MySQL | [InnoDB 并发领取任务](mysql/innodb-task-claim.md) | 行锁与死锁、RC 和 RR 的快照、条件更新、事务边界、`SKIP LOCKED` |
| Agent 开发 | [Worker 租约与任务回收](agent/worker-lease.md) | 崩溃恢复、心跳续租、接管和旧 worker 的写入 |
| Agent 开发 | [外部调用与邮件补发](agent/email-side-effects.md) | 幂等键、结果未知、迟到回调、按次记录、跳过补发 |
| Agent 开发 | [Agent 应用设计与人工复核](agent/application-design.md) | 公开岗位参考、固定流程与按需查规则、引用校验 |
| Agent 开发 | [工具调用与重试](agent/tool-calling.md) | Go 工具执行、超时预算、创建任务去重、跨服务复用幂等键 |

复习时先看场景，试着口述一遍，再对照时序和结论。

后续可以按 MySQL、Redis、Go、Scala、Spring Boot、Linux、Kubernetes、Agent 开发等主题增加笔记。每篇记录场景、结论和容易混淆的地方。复盘时可以围绕同一道题反复追问，等自己说「下一题」再切换。
