# PR #8714 确认版本验收

- 日期：2026-11-04；代码：`2f5c7d33223d7380edd36f760801d805ab73aa30`。
- 范围：Desktop 伙伴与群列表、电脑未读提示；#8715 话题/胶囊改色暂停，#8716 不改。
- 本次截图在提交前同内容工作区采集；提交后工作区干净，生产文件内容与提交一致。

## 最终显示

| 状态 | 展开 | 收起 |
| --- | --- | --- |
| Bot 私聊未读 | 绿点，保留时间 | 绿点 |
| 群普通未读 | 复用 NavigationCountBadge 灰色数字（99+）并保留时间 | 不显示普通未读点 |
| 群显式提及本人 | 蓝点，保留时间 | 蓝点 |
| 进行中 | 原处理摘要，不重复显示橙点；时间保留 | 橙色呼吸点 |
| 待处理 / 报错 | 青 / 红点，保留时间 | 青 / 红点 |

头像尺寸、状态点尺寸与位置、圆形选中描边沿用已确认版本。群蓝点与执行状态重叠时，本版本保留既有执行优先判据；不将其描述为老板原文中的新要求。未带显式提及的 Bot 回复本人尚无独立摘要判据，本 PR 没有补做消息关系识别。

## 清理与回归

- 清理收起条目中未消费的 unread 返回字段和过时注释；移除旧的“隐藏时间”断言，改为保留时间。保留撑住原行布局的占位节点，未借清理调整头像或行距。
- 补齐列表设计文档索引，更新 DESIGN.md 与专题规范，统一灰色数字、蓝点及时间说明。
- 选中远程 Cindy、generation 缺失但运行快照仍在时，旧代码无法显示处理摘要。最小回归先失败后通过；停止后恢复消息摘要。独立远程行、其他电脑运行仍覆盖。
- 对最新 origin/main 执行 merge-tree：无冲突；没有无必要地合并主干。

## 验证结果

| 命令 / 方法 | 结果 |
| --- | --- |
| `pnpm --filter desktop exec vitest run`（teammatesSection / botGroupSidebar / CindyDevicePicker / teammatesSectionSpacing / botListDisplay / BotGlancePopover，2 workers） | 6 文件，136 项通过，5.83 秒 |
| `pnpm --filter desktop run typecheck` | 通过 |
| `pnpm ui:check --page teammates-section --case all --theme all --engine electron` | 40/40 通过，38.6 秒 |
| `pnpm ui:check --changed --theme all --engine electron` | 134/134 通过，127.3 秒；device-picker / group-chat / teammate-glance / teammates-section |
| `pnpm check:dev-docs` / `pnpm check:design-colors --base-ref origin/main --worktree` / `git diff --check` | 通过 |
| `pnpm check:dco` | 4 个提交签名通过 |
| 完整 Cindy 开发版 | 来源与隔离预览 worktree 匹配，运行中组件已加载 remoteRunning 修复；没有抓取真实桌面 |

已目检主列表 Light/Dark 与概览，时间、灰色未读数、绿/蓝/红点显示正确。完整模拟场景原图见 [图册](GALLERY.md)，离线单文件见 [HTML 图册](gallery.html)。单页夹具不证明服务端读位、真实 Agent 提问或跨设备传输正确。

## 验证边界

- Windows 未实机目检；新 head 的全量 CI 另行运行。
- 前一 head `ec3bd8a7d1` 的 Windows shard 1 在未修改的 `VisionBridgeSectionRendering.test.tsx` 用例失败（预期保存调用但调用数为 0）；该设置模块不在本 PR diff。这里只记录，不能据此声称 Windows 全绿，也没有顺带修改设置模块。
- 本轮按影响面验证，没有重复整仓单测。首次全量命令曾因 Desktop 线程池 SIGSEGV 返回 1；相同范围以 2 个 fork worker 复跑通过 3,831 文件 / 65,852 测试。历史记录见原验收报告，不把复跑写成原命令全绿。
- 群内 thread/@ 胶囊继续沿用 main 蓝色；本 PR 不包含 #8715 改色，独立话题分支保留 Draft。
