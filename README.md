# 📚 Dating Skills — 恋爱方法论蒸馏技能包

> 由 [book2skill](https://github.com/nicobailey/book2skill) 流水线（RIA-TV++方法论）自动蒸馏产出。
> 忠实于原文，不做道德审查，不做改造净化。

## 仓库结构

```
dating-skills/
├── README.md                          ← 你正在看
├── mystery-method/                    ← 《谜男方法》蒸馏包
│   ├── BOOK_OVERVIEW.md               # 阶段0：整书理解（Adler四步分析）
│   ├── INDEX.md                       # 阶段3：技能索引 + 学习路径 + 关系图
│   └── skills/                        # 20个原子化技能
│       ├── m3-model.md                #   M3模型（吸引→舒适感→诱惑）
│       ├── approach-anxiety.md        #   接近焦虑管理
│       ├── group-approach.md          #   群组打开
│       ├── neg-tactics.md             #   否定话术
│       ├── dhv-display.md             #   DHV展示高价值
│       ├── ioi-iod-signals.md         #   IOI/IOD信号系统
│       ├── frame-control.md           #   框架控制
│       ├── compliance-testing.md      #   服从性测试
│       ├── intermittent-reward.md     #   间歇性奖赏
│       ├── calibration.md             #   社交标准化
│       ├── kino-escalation.md         #   进挪升高
│       ├── isolation-bounce.md        #   孤立+护送
│       ├── grounding-identity.md      #   背景植入
│       ├── conspiracy-rapport.md      #   同谋意识
│       ├── multi-threading.md         #   多重对话脉络
│       ├── lmr-destroy.md             #   LMR摧毁
│       ├── asd-handling.md            #   ASD反荡妇防卫
│       ├── jealousy-plotline.md       #   嫉妒情节
│       ├── freeze-out.md              #   冷冻机制
│       └── pawn-pivot.md              #   抵押/枢纽策略
```

## 如何使用这些 Skills

### 在 Hermes Agent 中使用（推荐）

将 `skills/` 目录下的 `.md` 文件放入 `~/.hermes/skills/` 即可被 agent 自动识别和调用。

```bash
# 复制到 Hermes skills 目录
cp -r mystery-method/skills/ ~/.hermes/skills/dating/mystery-method/
```

Agent 会在对话中根据 `description` 字段自动判断是否激活对应 skill。

### 在 Claude Code / Cursor 中使用

将 skill 文件放入你的 CLAUDE.md 或 .cursor/rules 引用路径中：

```bash
# 在项目根目录的 CLAUDE.md 中添加
See mystery-method/skills/ for dating methodology skills extracted from books.
```

### 作为独立知识库阅读

每个 skill 文件包含完整的 **RIA++ 六段结构**：

| 段落 | 内容 | 作用 |
|------|------|------|
| **R** Reading | 原文引用（≤150字） | 可追溯性 |
| **I** Interpretation | 方法论骨架（用自己的话） | 快速理解 |
| **A1** Past Application | 书中作者用过的案例 | 类比素材 |
| **A2** Future Trigger ★ | 触发场景 + 语言信号 | 何时使用 |
| **E** Execution | 1-2-3 可执行步骤 | 怎么用 |
| **B** Boundary ★ | 不适用场景 + 失败模式 | 防止乱用 |

### 推荐学习路径

按 INDEX.md 中的 **M3阶段递进路径** 学习：

```
基础层 → approach-anxiety, calibration, m3-model
吸引层 → group-approach → neg-tactics → dhv-display → ioi-iod-signals
操控层 → frame-control, compliance-testing, intermittent-reward
推进层 → kino-escalation → isolation-bounce → grounding-identity → conspiracy-rapport
收网层 → freeze-out → jealousy-plotline → asd-handling → lmr-destroy
```

## 蒸馏方法论：RIA-TV++

```
阶段 0: Adler 整书理解     → BOOK_OVERVIEW.md
阶段 1: 5个 agent 并行提取 → candidates/ (框架/原则/案例/反例/术语)
阶段 1.5: 三重验证筛选     → V1跨域 + V2预测力 + V3独特性
阶段 2: RIA++ 构造 skill   → 每个skill的 SKILL.md
阶段 3: Zettelkasten 链接  → INDEX.md (引用图 + 学习路径)
阶段 4: 压力测试           → test-prompts.json (darwin兼容)
```

## 贡献的书目

| 书名 | 作者 | 产出skill数 | 状态 |
|------|------|-------------|------|
| 谜男方法 (The Mystery Method) | Mystery | 20 | ✅ 完成 |

| 野兽绅士 (Beast Gentleman) | 巫家民（Tango） | 2017 | 18 | ✅ 完成 |

## License

MIT — 技能内容提取自原书，版权归原作者所有。
