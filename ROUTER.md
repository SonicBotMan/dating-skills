# 场景路由表 (Scene Router)

> 给 AI 助手用: 用户描述一个处境, 从下表定位技能文件, 读 2-3 个候选再组合回复。
> 全部路径相对仓库根, 每个场景给出不同流派的多个候选——**先读多个候选, 再按用户处境组合成 2-3 种风格回复**(调皮/暧昧/直接)。
> 本表由内容实测生成 (2026-09-03), 19 条路由全部验证存在。

## 她发来一条消息只回「嗯」，聊天接不住

触发词: 嗯, 回复, 接不住, 聊天, 冷回复

| 优先级 | 技能文件 | 流派 |
|---|---|---|
| ★ 主 | `beast-gentleman/skills/push-pull-dynamics.md` | 推拉法则/话术 |
| 候选1 | `the-game-neil/skills/push-pull.md` | 推拉法 |
| 候选2 | `fanchen-scripts/skills/push-pull-technique.md` | 梵尘推拉技巧 |

## 第一次约会，不知道聊什么

触发词: 第一次约会, 初次约会, 约会, 聊什么, date

| 优先级 | 技能文件 | 流派 |
|---|---|---|
| ★ 主 | `devil-chat/skills/first-date-assessment.md` | 第一次约会评估 |
| 候选1 | `beast-gentleman/skills/date-flow-design.md` | 约会流程设计 |
| 候选2 | `cold-reading-book/skills/cup-distance-technique.md` | 冷读测距 |

## 约会冷场，空气突然安静

触发词: 冷场, 安静, 没话题, 尴尬

| 优先级 | 技能文件 | 流派 |
|---|---|---|
| ★ 主 | `mystery-method/skills/multi-threading.md` | 多重对话脉络 |
| 候选1 | `cai-kangyong-talk/skills/topic-management.md` | 话题管理 |
| 候选2 | `cai-kangyong-talk/skills/silence-value.md` | 沉默的价值 |

## 她问「你是不是渣男」/关系测试

触发词: 渣男, 测试, 服从性, 框架

| 优先级 | 技能文件 | 流派 |
|---|---|---|
| ★ 主 | `extreme-scripts/skills/shit-test-coping.md` | 废物测试应对 |
| 候选1 | `mystery-method/skills/frame-control.md` | 框架控制 |
| 候选2 | `mystery-method/skills/compliance-testing.md` | 服从性测试 |

## 想牵手/接吻，不知道时机

触发词: 牵手, 接吻, 亲她, 升级, kino, 进挪, IOI, 时机

| 优先级 | 技能文件 | 流派 |
|---|---|---|
| ★ 主 | `mystery-method/skills/kino-escalation.md` | 进挪升高 |
| 候选1 | `mystery-method/skills/ioi-iod-signals.md` | IOI/IOD 信号 |
| 候选2 | `the-game-neil/skills/kino-touch.md` | 进挪/肢体接触 |
| 候选3 | `beast-gentleman/skills/kino-escalation-bg.md` | 渐进式身体接触 |

## 被已读不回/她突然消失

触发词: 已读, 不回, 消失, 冷冻, 断联

| 优先级 | 技能文件 | 流派 |
|---|---|---|
| ★ 主 | `mystery-method/skills/freeze-out.md` | 冷冻机制 |
| 候选1 | `mystery-method/skills/intermittent-reward.md` | 间歇性奖赏 |
| 候选2 | `fanchen-scripts/skills/push-pull-technique.md` | 梵尘推拉技巧 |

## 使用方式

1. 匹配用户处境到上面的场景 (按触发词模糊匹配)
2. 依次读取该场景的 ★主技能 + 至少 1 个候选技能
3. 综合不同流派, 给用户 2-3 种风格的回复建议 (如: 调皮型 / 暧昧型 / 直接型), 并说明各自的适用情境
4. 若场景不在表中, 按 `git grep -l '<处境关键词>' */skills/` 检索, 或读对应书的 `INDEX.md`

## 边界

涉及未成年、真实骚扰、非法行为时拒绝使用本库。技能内容忠实提取自原书, 使用者自担判断。