# Prompt Aspect Checklist

> Purpose: Summary of what the prompt explicitly asks the LLM to analyze and check for each aspect.

## 1) Quick Tear Sheet

**Focus**
- Identity disambiguation
- Indication map
- SOC benchmarking
- Efficacy readouts
- Safety/tolerability
- Clinical positioning
- Regulatory & evidence quality
- Commercial sketch
- Go/No-Go decision

**LLM required checks**
- Drug name normalization (generic/brand/code) and sponsor
- Mechanism/class/modality/route
- Approved indications by region + approval dates
- Key late-stage trials (Phase 2/3) + IDs
- SOC guideline version/date/issuer
- Trial endpoints and values with context
- Conflicts among sources and resolution
- Company-only claims flagged

---

## 2) Trial Progress & Reliability

**Focus**
- Trial inventory
- Original design baseline
- Protocol change log
- Enrollment dynamics
- Dropout/missingness
- Analysis population integrity
- Data maturity/readout quality
- Historical precedents mapping
- Red flags & reliability verdict

**LLM required checks**
- Registry history versions and update dates
- Amendments: endpoints/sample size/inclusion changes
- Timing of changes vs enrollment/unblinding
- Enrollment trajectory vs plan
- Geographic/site concentration risks
- Differential dropout by arm
- Missing data handling (censoring/imputation)
- ITT/mITT/PP definitions stability
- BICR vs investigator consistency
- Readout maturity (events/follow-up)

---

## 3) Efficacy

**Focus**
- Indication anchoring
- Comparator set (SOC/target/mechanism/future)
- Structured efficacy extraction
- Cross-trial comparability
- Differentiation labeling
- Future SOC stress test

**LLM required checks**
- Anchors reflect most material indications/lines
- Comparator completeness & relevance
- Endpoint definitions by disease area
- HR/CI/p-values aligned with sources
- Population/biomarker differences in comparisons
- Follow-up maturity & OS confounding
- Evidence grade vs data strength

---

## 4) Safety

**Focus**
- Key clinical scenarios
- Comparator safety baselines
- AE profile extraction
- Real-world usability inference
- Combination feasibility
- Long-term safety maturity

**LLM required checks**
- AE tables from primary sources
- TEAE vs TRAE definitions
- Grade ≥3/SAE/Discontinuation rates
- Dose mods & exposure duration
- Key organ toxicities flagged
- Combo toxicity delta vs benchmark
- Long-term signals (≥12/24m)
- Drift across disclosures

---

## 5) Ongoing Clinical Trials

**Focus**
- Full trial universe
- Normalization & de-dup
- Development momentum
- Catalyst identification
- Catalyst scoring
- Timeline (0–6/6–12/12–24m)
- Pre-mortem risks

**LLM required checks**
- Registry fields accuracy
- Company guidance vs registry alignment
- Estimated dates labeled & justified
- Event-driven assumptions
- Trial status changes
- Catalyst materiality rationale

---

## 6) Strategies

**Focus**
- Current strategy map
- Internal option space
- Constraints (bio/clinical/competition)
- Historical precedents
- Strategy fit scoring
- Alternative strategy proposals
- Pre-mortem failure scenarios

**LLM required checks**
- Indication/line sequencing logic
- Mono vs combo rationale
- Endpoint/regulatory fit
- Precedent relevance & validity
- Competitive timing vs peers
- Alternative strategies feasibility

---

## 7) Competitive Landscape

**Focus**
- Ecosystem boundary definition
- Landscape inventory
- Scoring matrix
- Evidence-fed scoring
- Comparability control
- Tiering/ranking narrative
- Future SOC dynamics

**LLM required checks**
- Inclusion/exclusion rules soundness
- Competitor list completeness
- Scoring rubric consistent
- Evidence sources are primary
- Comparability bias explicitly noted
- Ranking range justified

---

## Global Rules (LLM must enforce)

- Cutoff date enforced
- Each key claim has a link
- Conflicts resolved with trust hierarchy
- Unknown used when data missing
- Company-only info flagged
- Output format (A: one-page sheet + B: evidence appendix)

---\n+
# 提示词维度核对清单

> 用途：汇总 prompt 明确要求 LLM 执行的分析与核对点。

## 1) 快速是否值得深挖

**切入点**
- 药物身份消歧
- 适应症地图
- 标准治疗基准
- 疗效读出
- 安全性/耐受性
- 临床定位
- 监管与证据质量
- 商业速写
- 是否值得深挖判定

**模型需核对项**
- 通用名/商品名/代号及持有人是否一致
- 机制/类别/形式/给药方式是否明确且来源可靠
- 各地区已批适应症与日期是否完整
- 关键后期试验与试验ID是否齐全
- SOC指南版本/日期/发布机构是否准确
- 关键终点数值与人群/时间点口径
- 多来源冲突是否解释并排序
- 仅公司口径是否标注并提示缺口

---

## 2) 试验进展与可信度

**切入点**
- 试验清单
- 原始设计基线
- 方案变更日志
- 招募动态
- 掉队与缺失
- 分析集完整性
- 数据成熟度与读出质量
- 历史先例映射
- 红旗清单与可信度裁决

**模型需核对项**
- 注册库历史版本与更新时间
- 终点/样本量/入排变更是否有证据
- 变更时间与入组/揭盲关系
- 实际入组是否偏离原计划
- 地区/中心集中风险是否提示
- 治疗组间差异性脱落
- 缺失数据处理策略
- 分析集定义是否稳定
- 盲评与研究者评估一致性
- 事件数/随访是否成熟

---

## 3) 疗效差异化

**切入点**
- 适应症锚点选择
- 对照集合构建
- 疗效读出结构化抽取
- 跨试验可比性评估
- 差异化结论标签
- 未来SOC压力测试

**模型需核对项**
- 锚点是否为最关键适应症/线别
- 对照是否完整且相关
- 终点是否匹配疾病领域
- 统计值是否与来源一致
- 人群/标志物差异是否说明
- 随访成熟度及OS混杂因素
- 证据等级是否合理

---

## 4) 安全性与可用性

**切入点**
- 关键场景定义
- 对照安全性基准
- 不良事件抽取
- 真实世界可用性推断
- 联合可行性
- 长期安全性成熟度

**模型需核对项**
- AE表是否来自论文/标签/会议
- TEAE/TRAE口径是否明确
- 严重AE/SAE/停药率是否齐全
- 剂量调整与暴露时间是否披露
- 关键器官毒性是否识别
- 联合毒性增量是否量化
- 长期信号是否有数据支撑
- 不同披露版本是否一致

---

## 5) 在研试验与催化剂

**切入点**
- 试验全量清单
- 去重与字段对齐
- 研发动能判断
- 催化剂识别
- 催化剂含金量评分
- 时间线
- 风险覆盖

**模型需核对项**
- 注册库字段是否准确
- 公司时间线是否与注册库对齐
- 估算日期是否有依据
- 事件驱动假设是否合理
- 试验状态变更是否更新
- 催化剂评分理由是否清晰

---

## 6) 开发策略

**切入点**
- 当前策略图谱
- 可选路径空间
- 约束因素
- 同类先例
- 策略适配度评分
- 备选策略
- 失败推演

**模型需核对项**
- 适应症与线别排序是否合理
- 单药/联合逻辑是否清晰
- 终点与监管可接受性
- 先例是否真正同类
- 读出时间线是否落后竞品
- 备选策略可行性

---

## 7) 竞争格局

**切入点**
- 生态边界定义
- 竞争者清单
- 评分矩阵
- 证据驱动评分
- 可比性控制
- 分层与排名叙事
- 未来SOC动态

**模型需核对项**
- 边界规则是否合理
- 竞争者是否漏列
- 评分标准是否一致
- 关键数据是否来源于一手证据
- 偏倚方向是否明确
- 排名区间是否有依据

---

## 全局规则（模型必须执行）

- 截止日期限制是否严格执行
- 关键结论是否都有链接
- 冲突是否按可信度排序裁决
- 缺数据是否写Unknown
- 仅公司口径是否标注
- 输出格式是否符合A/B结构
