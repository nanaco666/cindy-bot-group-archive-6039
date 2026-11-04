# PR #8714 复核补充

当前修复提交：`4ef457eabd55f65db77d95a4a37312fd7950a5ee`。2026-11-04。

- 两条运行提示评论为同一根因：合并行汇总其他电脑的运行状态，却只显示当前电脑的消息摘要。
- 当前电脑空闲、其他电脑运行时显示“运行电脑 · 处理状态”；当前电脑也运行时仍保留当前摘要。不补回展开橙点，不改变选择或打开路由；结束后恢复原消息。
- 同步 DESIGN.md 三处旧 Desktop 结论：点击目标／选中态、普通未读和电脑未读颜色。Mobile、群话题蓝色规则、另两张 PR 保持不变。

## 验证

新增用例修复前 3 项失败、1 项通过；修复后相关 4 文件／109 项单测通过。Desktop typecheck、10/10 个明暗主题 Electron UI 变体、文档检查、设计清单、颜色审计和 diff 检查均通过。

本轮按影响面验证，未重复整仓单测；首次提交的完整测试及 SIGSEGV／forks 复跑记录仍见原报告。当前 head 的 CI 和自动审查需独立观察，不沿用旧 head 的绿色或 4/5。

## 真实组件截图

本地真实 Electron 组件＋示例运行镜像；不是实际网络跨电脑传输验收。未改数据协议、宿主执行逻辑或动画。

### local-working-remote-selected.dark

![真实组件完整截图](local-working-remote-selected.dark.png)

### local-working-remote-selected.light

![真实组件完整截图](local-working-remote-selected.light.png)

### other-computer-running-mirror.dark

![真实组件完整截图](other-computer-running-mirror.dark.png)

### other-computer-running-mirror.light

![真实组件完整截图](other-computer-running-mirror.light.png)

### other-computer-running.dark

![真实组件完整截图](other-computer-running.dark.png)

### other-computer-running.light

![真实组件完整截图](other-computer-running.light.png)
