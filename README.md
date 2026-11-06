## Hi there 👋

软件工程学术型硕士（安徽理工大学 · 计算机科学与工程学院），研究方向是**知识图谱驱动的软件分析与测试** ——
把 C 程序的函数调用路径建成带类型的知识图，再做冗余约简与不可行路径的保守筛查。

> ### ⚠️ 账号说明
> 我在 GitHub 上**只有一个账号：`William-Practice`（即本账号）**。
> 同名的 `Wuruiyang` 账号**与本人无关**，请勿混淆。
>
> （GitHub 用户 ID 是永久唯一的：本账号为 `191301418`。）

---

### 📄 论文

**Knowledge Graph-Based Generation of Function Call Path in Software Systems**

Ruiyang Wu, Changqing Wei (corresponding), Dunwei Gong, Xiangjuan Yao

*第一作者 · 拟投 Information and Software Technology（IST, CCF-B / 中科院 2 区）*

在 **8 个 C 对象**上保留 **3,923 条**函数级调用路径，相较 **35,906 条**语句级基线体量低 **89.1%**
（跨粒度参照，非等量约简），同时完整覆盖 **6,190 条**可达调用边（静态调用边的 **94.2%**）。
三个对比选择器分别多保留 45–440 条路径，**仅 PathKG 能证明所选路径数已达最小**。
中位选路耗时 **0.58 s**（PE-guided 12.16 s，**21.1×**），端到端流水线 **147 s**。

→ 基准包与复现材料：[c-path-analysis-benchmark](https://github.com/William-Practice/c-path-analysis-benchmark)

### 📦 主要项目

| 仓库 | 说明 |
|---|---|
| [c-path-analysis-benchmark](https://github.com/William-Practice/c-path-analysis-benchmark) | **论文配套基准包**（MIT）：受控 C 测试对象、调用路径实验数据与复现脚本 |
| [taxi-realtime-warehouse](https://github.com/William-Practice/taxi-realtime-warehouse) | **出租车 GPS 实时数仓**：Flink CDC → Apache Paimon 湖仓（ODS/DIM/DWM/DWS）→ ADS → WebSocket 实时大屏。对一套早期课程栈的**现代化改造**：湖由 Hudi 换 Paimon，OLAP 由 ClickHouse 换 Paimon 内嵌查询 + MySQL serving（受 3.8 GB 内存约束），环境搭建、选型取舍、链路排障与调优验证由本人完成 |
| [knowledge-base-rag](https://github.com/William-Practice/knowledge-base-rag) | **RAG 知识库问答**：5 层架构（Query 重写 → 向量召回 Top10 → Rerank 精排 Top3 → LLM 生成 → FastAPI 服务）· 课程作业二次实现 |

### 🛠 技术栈

| 方向 | 工具 |
|---|---|
| **研究** | 知识图谱（Neo4j）· 静态分析（Clang AST）· 符号执行（KLEE）· 精确求解（MILP / HiGHS）· 启发式搜索（NSGA-II） |
| **数据系统** | Flink CDC · Apache Paimon · Kafka · Hive · Spark · HDFS |
| **工程** | Python · Java · FastAPI · Spring Boot · Docker · Git / GitHub Actions · LaTeX |

---

📫 **2025201502@aust.edu.cn**

🎯 2027 年暑期实习 —— 软件工程 / 数据平台 / 智能软件分析方向
