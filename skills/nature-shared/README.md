# `nature-shared/` - manuscript-* 与 reviewer 的共享支持包

这个目录是一个可安装但不应单独触发的支持包。它保存canonical manuscript-* suite 与 nature-reviewer 共同依赖的公共定义与参考材料，避免在不同技能目录中重复维护同一套内容。它作为内部依赖保留，不作为独立写作入口。

同级技能会通过 `manifest.yaml` 中的相对路径引用这里的文件，例如：

```yaml
always_load:
  - ../nature-shared/core/reader-workflow.md
```

## 当前内容

| 文件 | 使用方 |
|---|---|
| `core/reader-workflow.md` | `manuscript-polishing`, `manuscript-workflow` |
| `core/paper-type-taxonomy.md` | `manuscript-polishing`, `manuscript-workflow` |
| `core/ethics.md` | `manuscript-polishing`, `manuscript-workflow` |
| `core/research-compliance.md` | `manuscript-workflow` 及需要 Nature Portfolio 专项合规检查的技能 |
| `core/terminology-ledger.md` | `manuscript-polishing`, `manuscript-workflow` 及其它需要术语账本的消费者 |
| `core/consistency-sweep.md` | `manuscript-polishing`, `nature-reviewer` and other review consumers |
| `core/main-text-discipline.md` | `manuscript-workflow`, `manuscript-polishing` and revision consumers |
| `core/nature-results-discussion.md` | `manuscript-workflow`, `manuscript-polishing` 通用的 Nature / Nature Portfolio Results claim 递进与 Discussion 综合（来自 NMI 与旗舰 Nature 已发表论文语料归纳，非官方规则） |
| `core/discussion-argument-language.md` | `manuscript-workflow`, `manuscript-polishing` 通用的 Discussion 功能链、反向漏斗、证据强度与情态动词、局限和未来工作审计（写作指导，非期刊官方规则） |
| `core/nature-introduction.md` | `manuscript-workflow`, `manuscript-polishing` 通用的 Nature / Nature Portfolio 问题漏斗、精确 gap 与 Introduction–Results 对齐（最初来自 NMI 语料归纳，非官方规则） |
| `core/nature-abstract.md` | `manuscript-workflow`, `manuscript-polishing` 通用的 Nature / Nature Portfolio 发现中心型摘要证据链、claim 层级与数字取舍（最初来自 NMI 语料归纳，非官方规则） |
| `journal-formats/nat-comms.md` | `manuscript-polishing`, `manuscript-workflow` |
| `journal-formats/nature.md` | `manuscript-workflow` 及需要旗舰 `Nature Article` 精确投稿规则的技能 |
| `journal-formats/nature-machine-intelligence.md` | NMI 投稿的写作、润色、图表、数据与统计工作流 |

`scripts/check_consistency.py` 为一致性扫描提供机械初筛，可报告术语变体、同值不同精度和等值长度单位混用。输出是待人工核对的风险提示，不会自动改稿。

## 什么时候把文件放到这里

只有当**两个或更多技能**需要复用同一份内容时，才把文件放入 `nature-shared/`。如果内容只服务于一个技能，应保留在该技能自己的 `static/` 或 `references/` 目录中。

## 什么时候保持技能内局部内容

共享层只放**定义和参考材料**，例如论文类型分类、读者工作流、伦理规则或术语表。具体技能如何诊断、起草、修改或输出结果，仍应保留在各自的 `static/fragments/` 中。多个技能可以复用同一套论文类型分类，但在其上执行不同的任务逻辑。

## 与其它技能的关系

`nature-shared/` 不是独立工作流，而是被 canonical manuscript-* skills 与 nature-reviewer 按需读取的公共依赖包。
