# Startup Strategy Skill

给创业公司的战略梳理技能。把业务、增长、团队、资金、对外合作和招聘连起来，帮助创始人选择下一步，并形成能复盘的行动。

作者：KenichiXXX｜版本：0.1.0

## 它会交付什么

- 一页战略摘要：当前卡点、推荐方案、其他选项、暂缓事项和决策。
- `business-state.md`：公司事实、未知项与证据链接，保存到使用者自己的工作目录。
- 执行表：最终负责人、日期、资源、验收证据、依赖和继续/暂停条件。
- 按需展开招聘成果定义、合作试点或资金里程碑。

它不会把目标当实际收入，把意向资金当现金，把岗位清单当已到岗团队。数据不足时给条件性建议，保留影响决定的未知项。

## 使用示例

```text
用 startup-strategy 做一次全局梳理。先读取我提供的材料，
找出当前最关键的业务约束，比较不同选择，再给下一阶段行动。
```

```text
我们想扩大销售团队。用 startup-strategy 判断卡点是否需要招聘，
结合现金、销售周期和交付容量，给岗位成果、成本和验证计划。
```

```text
用 startup-strategy 评估这个渠道合作：双方为什么合作、
什么是新增价值、谁负责交付，以及怎样用小试点验证。
```

## 安装到 Codex

本仓库的可安装目录是 `skills/startup-strategy/`，安装后文件夹名称应为 `startup-strategy`。将该目录放到 Codex 的技能目录（默认 `~/.codex/skills/`），已有同名技能时先检查，避免覆盖。下一轮对话可用 `$startup-strategy` 或自然语言调用。

也可以向支持安装技能的 Agent 发出这条指令：

```text
请从 https://github.com/KenichiXXX/startup-strategy-skill
安装 skills/startup-strategy 目录里的技能，保留该目录内的 LICENSE。
若已有同名技能，先检查现有版本，不要直接覆盖。
```

其他支持 `SKILL.md` 的 Agent 可将同一目录安装到各自技能目录；尚未在其他宿主中验证。无需 API key、账号登录或运行服务。

## 文件结构

```text
skills/startup-strategy/
  SKILL.md
  agents/openai.yaml
  references/strategy-domains.md
  references/output-template.md
examples/fictional-b2b-case.md
evals/scenarios.md
```

示例是完全虚构的练习输入与示范推演，不是客户成果或效果证明。`evals/scenarios.md` 定义验收场景；不能据此宣称跨模型验证通过。

## 设计来源与边界

由仓库维护者提出产品方向。阅读 RedSkill 分发的 `wzceo-skill@1.0.0`（内部名称 `startup-daily`）后，参考其“先整理公司状态，再做行动梳理”的工作思路。

本仓库的说明、问题参考、模板和虚构案例均为此次独立撰写；不包含原技能的正文或看板模板，也不包含任何真实公司的业务数据、合同、客户清单或私人档案。不宣称与 RedSkill、小红书或原技能作者存在合作、授权或背书。

Skill 使用者的公司记录应保存在自己的业务目录。发布仓库前审查文件与 Git 历史；`.gitignore` 只防止后续意外加入，不负责撤回已经发布的数据。

## 版本与许可

0.1.0 是可试用初稿，已进行本地结构检查和作者场景推演；尚未完成独立 Agent 行为测试、多个真实公司试用或跨宿主验证。

本仓库独立编写的内容采用 [MIT License](LICENSE)。可安装技能目录也附有相同许可文本，单独分发该目录时请保留。
