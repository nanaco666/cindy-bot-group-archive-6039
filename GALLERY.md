# Bot／群 UI 状态图册（公开版）

30 组场景、60 个明暗截图视图。来源为 2026-11-03 验收，2026-11-04 核对当前提交后汇总。真实账号截图已移除，原始像素未改色；电脑近况仅保留相关区域。

[验收报告](REPORT.md) · [交互图册 HTML（下载后打开）](gallery.html)

提交：列表 `358e9a3909`；话题 `336ba086fd`；委派 `4940dc6611`。分隔线外观摘录单独标明，不作为完整消息流运行证据。

## 展开列表

### 运行、待处理、完成未读、普通未读、错误

从上到下：运行只保留摘要；待处理青点；完成未读和普通未读绿点；错误红点。Writer 为选中行。

真实组件 · 示例数据

**浅色**

<img src="images/im0.png" width="440" alt="运行、待处理、完成未读、普通未读、错误">

**深色**

<img src="images/im2.png" width="440" alt="运行、待处理、完成未读、普通未读、错误">

<details><summary>查看完整场景截图</summary>

![浅色](images/im1.png)

![深色](images/im3.png)

</details>

### 空闲／已读与时间

没有执行状态或未读时不显示点，保留时间。这里同时展示未选中和选中行。

真实组件 · 示例数据

**浅色**

<img src="images/im4.png" width="440" alt="空闲／已读与时间">

**深色**

<img src="images/im6.png" width="440" alt="空闲／已读与时间">

<details><summary>查看完整场景截图</summary>

![浅色](images/im5.png)

![深色](images/im7.png)

</details>

### 读位确认后的变化

模拟读位确认后，Researcher 的绿点消失；待处理和错误点保留。此图不证明服务端已读同步。

真实组件 · 示例数据

**浅色**

<img src="images/im8.png" width="440" alt="读位确认后的变化">

**深色**

<img src="images/im10.png" width="440" alt="读位确认后的变化">

<details><summary>查看完整场景截图</summary>

![浅色](images/im9.png)

![深色](images/im11.png)

</details>

### 群与 Bot 混排

保留原群头像拼合，不增加群类型小图标；展开的进行中群没有重复橙点。

真实组件 · 示例数据

**浅色**

<img src="images/im12.png" width="440" alt="群与 Bot 混排">

**深色**

<img src="images/im14.png" width="440" alt="群与 Bot 混排">

<details><summary>查看完整场景截图</summary>

![浅色](images/im13.png)

![深色](images/im15.png)

</details>

## 收起头像

### 五类状态＋圆形选中

从左到右：运行橙、待处理青、完成未读绿、普通未读绿、错误红。第二个头像选中，点色保持。

真实组件 · 示例数据

**浅色**

<img src="images/im16.png" width="440" alt="五类状态＋圆形选中">

**深色**

<img src="images/im18.png" width="440" alt="五类状态＋圆形选中">

<details><summary>查看完整场景截图</summary>

![浅色](images/im17.png)

![深色](images/im19.png)

</details>

### 空闲、选中与 +N

头像和 +N 内圈均为 36px；选中使用外描边，点击区 40px、横向间距 4px。

真实组件 · 示例数据

**浅色**

<img src="images/im20.png" width="440" alt="空闲、选中与 +N">

**深色**

<img src="images/im22.png" width="440" alt="空闲、选中与 +N">

<details><summary>查看完整场景截图</summary>

![浅色](images/im21.png)

![深色](images/im23.png)

</details>

### 群有提及：运行与未读

提及不覆盖执行状态：运行仍为橙点，其他未读为绿点。列表头像上不额外显示 @ 或数字。

真实组件 · 示例数据

**浅色**

<img src="images/im24.png" width="440" alt="群有提及：运行与未读">

**深色**

<img src="images/im26.png" width="440" alt="群有提及：运行与未读">

<details><summary>查看完整场景截图</summary>

![浅色](images/im25.png)

![深色](images/im27.png)

</details>

### 没有提及时的外观

同一组群头像，无提及标记；圆形描边、头像和右下状态点几何不变。

真实组件 · 示例数据

**浅色**

<img src="images/im28.png" width="440" alt="没有提及时的外观">

**深色**

<img src="images/im30.png" width="440" alt="没有提及时的外观">

<details><summary>查看完整场景截图</summary>

![浅色](images/im29.png)

![深色](images/im31.png)

</details>

## 1–5 人选中

### 1 人群头像选中

五个群按 1、2、3、4、5 人排列，本图选中 1 人群。使用真实预设头像，保留头像拼合。

真实组件 · 示例数据

**浅色**

<img src="images/im32.png" width="440" alt="1 人群头像选中">

**深色**

<img src="images/im34.png" width="440" alt="1 人群头像选中">

<details><summary>查看完整场景截图</summary>

![浅色](images/im33.png)

![深色](images/im35.png)

</details>

### 2 人群头像选中

五个群按 1、2、3、4、5 人排列，本图选中 2 人群。使用真实预设头像，保留头像拼合。

真实组件 · 示例数据

**浅色**

<img src="images/im36.png" width="440" alt="2 人群头像选中">

**深色**

<img src="images/im38.png" width="440" alt="2 人群头像选中">

<details><summary>查看完整场景截图</summary>

![浅色](images/im37.png)

![深色](images/im39.png)

</details>

### 3 人群头像选中

五个群按 1、2、3、4、5 人排列，本图选中 3 人群。使用真实预设头像，保留头像拼合。

真实组件 · 示例数据

**浅色**

<img src="images/im40.png" width="440" alt="3 人群头像选中">

**深色**

<img src="images/im42.png" width="440" alt="3 人群头像选中">

<details><summary>查看完整场景截图</summary>

![浅色](images/im41.png)

![深色](images/im43.png)

</details>

### 4 人群头像选中

五个群按 1、2、3、4、5 人排列，本图选中 4 人群。使用真实预设头像，保留头像拼合。

真实组件 · 示例数据

**浅色**

<img src="images/im44.png" width="440" alt="4 人群头像选中">

**深色**

<img src="images/im46.png" width="440" alt="4 人群头像选中">

<details><summary>查看完整场景截图</summary>

![浅色](images/im45.png)

![深色](images/im47.png)

</details>

### 5 人群头像选中

五个群按 1、2、3、4、5 人排列，本图选中 5 人群。使用真实预设头像，保留头像拼合。

真实组件 · 示例数据

**浅色**

<img src="images/im48.png" width="440" alt="5 人群头像选中">

**深色**

<img src="images/im50.png" width="440" alt="5 人群头像选中">

<details><summary>查看完整场景截图</summary>

![浅色](images/im49.png)

![深色](images/im51.png)

</details>

## 设备与近况

### 设备菜单：本机选中

未读设备使用绿点；离线文字和当前设备勾选保留。

真实组件 · 示例数据

**浅色**

<img src="images/im52.png" width="440" alt="设备菜单：本机选中">

**深色**

<img src="images/im54.png" width="440" alt="设备菜单：本机选中">

<details><summary>查看完整场景截图</summary>

![浅色](images/im53.png)

![深色](images/im55.png)

</details>

### 设备菜单：长名称／远程选中

设备长名称截断，离线说明、未读点和当前勾选继续显示。

真实组件 · 示例数据

**浅色**

<img src="images/im56.png" width="440" alt="设备菜单：长名称／远程选中">

**深色**

<img src="images/im58.png" width="440" alt="设备菜单：长名称／远程选中">

<details><summary>查看完整场景截图</summary>

![浅色](images/im57.png)

![深色](images/im59.png)

</details>

### 近况中的电脑未读

真实组件的电脑区域：当前电脑勾选，其他电脑未读绿点。公开图已裁掉无关的样本待办区域。

真实组件 · 示例数据 · 公开裁剪

**浅色**

<img src="images/public-computer-light.png" width="440" alt="近况中的电脑未读">

**深色**

<img src="images/public-computer-dark.png" width="440" alt="近况中的电脑未读">

<details><summary>查看完整场景截图</summary>

![浅色](images/public-computer-light.png)

![深色](images/public-computer-dark.png)

</details>

## 话题与胶囊

### 群话题与私聊话题入口

群话题保留回复数、未读回复数与提及文字；私聊话题保留“有新回复”。已有未读点改为绿色。

真实组件 · 示例数据

**浅色**

<img src="images/im64.png" width="440" alt="群话题与私聊话题入口">

**深色**

<img src="images/im66.png" width="440" alt="群话题与私聊话题入口">

<details><summary>查看完整场景截图</summary>

![浅色](images/im65.png)

![深色](images/im67.png)

</details>

### 胶囊收起状态

话题新回复与提及提示，保持原胶囊结构、数量、关闭按钮，仅统一状态点颜色。

真实组件 · 示例数据

**浅色**

<img src="images/im68.png" width="440" alt="胶囊收起状态">

**深色**

<img src="images/im69.png" width="440" alt="胶囊收起状态">

<details><summary>查看完整场景截图</summary>

![浅色](images/im65.png)

![深色](images/im67.png)

</details>

### 话题胶囊展开

打开后的话题列表、原有操作和绿点。

真实组件 · 示例数据

**浅色**

<img src="images/im70.png" width="440" alt="话题胶囊展开">

**深色**

<img src="images/im72.png" width="440" alt="话题胶囊展开">

<details><summary>查看完整场景截图</summary>

![浅色](images/im71.png)

![深色](images/im73.png)

</details>

### 提及胶囊展开

“@ 我的消息”列表及全部标为已读入口；绿色只替换原提示点。

真实组件 · 示例数据

**浅色**

<img src="images/im74.png" width="440" alt="提及胶囊展开">

**深色**

<img src="images/im76.png" width="440" alt="提及胶囊展开">

<details><summary>查看完整场景截图</summary>

![浅色](images/im75.png)

![深色](images/im77.png)

</details>

### 分隔线对照

上：Bot 主消息流 NEW 分隔线保持 main 原样。下：群话题新回复点为绿色。这里为原组件 JSX 摘录截图，不是完整消息流运行证据。

分隔线外观摘录 · 已标明边界

**浅色**

<img src="images/im78.png" width="440" alt="分隔线对照">

**深色**

<img src="images/im79.png" width="440" alt="分隔线对照">

<details><summary>查看完整场景截图</summary>

![浅色](images/im65.png)

![深色](images/im67.png)

</details>

### 真实群话题面板

原消息和回复区域的实际布局；当前样本为普通回复分隔线。与上方“新回复”摘录区分。

真实组件 · 示例数据

**浅色**

<img src="images/im80.png" width="440" alt="真实群话题面板">

**深色**

<img src="images/im82.png" width="440" alt="真实群话题面板">

<details><summary>查看完整场景截图</summary>

![浅色](images/im81.png)

![深色](images/im83.png)

</details>

### 真实私聊话题面板

私聊话题的实际面板与输入区域，展示当前整体布局。

真实组件 · 示例数据

**浅色**

<img src="images/im84.png" width="440" alt="真实私聊话题面板">

**深色**

<img src="images/im86.png" width="440" alt="真实私聊话题面板">

<details><summary>查看完整场景截图</summary>

![浅色](images/im85.png)

![深色](images/im87.png)

</details>

### 话题失败状态

真实组件的失败样本；保留原有错误与操作，不在此次统一中重设计。

真实组件 · 示例数据

**浅色**

<img src="images/im88.png" width="440" alt="话题失败状态">

**深色**

<img src="images/im90.png" width="440" alt="话题失败状态">

<details><summary>查看完整场景截图</summary>

![浅色](images/im89.png)

![深色](images/im91.png)

</details>

## 群委派

### 即将开始

橙色呼吸点，保留“正在开始”、打开与停止操作。 局部聚焦左侧状态；右侧操作见完整原图。

真实组件 · 示例数据

**浅色**

<img src="images/im92.png" width="440" alt="即将开始">

**深色**

<img src="images/im94.png" width="440" alt="即将开始">

<details><summary>查看完整场景截图</summary>

![浅色](images/im93.png)

![深色](images/im95.png)

</details>

### 进行中

橙色呼吸点，保留处理中摘要、补一句和停止。 局部聚焦左侧状态；右侧操作见完整原图。

真实组件 · 示例数据

**浅色**

<img src="images/im96.png" width="440" alt="进行中">

**深色**

<img src="images/im97.png" width="440" alt="进行中">

<details><summary>查看完整场景截图</summary>

![浅色](images/im93.png)

![深色](images/im95.png)

</details>

### 待处理

青色点，保留等待确认与查看操作。 局部聚焦左侧状态；右侧操作见完整原图。

真实组件 · 示例数据

**浅色**

<img src="images/im98.png" width="440" alt="待处理">

**深色**

<img src="images/im99.png" width="440" alt="待处理">

<details><summary>查看完整场景截图</summary>

![浅色](images/im93.png)

![深色](images/im95.png)

</details>

### 已完成

绿色点，保留结果摘要、展开结果和打开任务。 局部聚焦左侧状态；右侧操作见完整原图。

真实组件 · 示例数据

**浅色**

<img src="images/im100.png" width="440" alt="已完成">

**深色**

<img src="images/im101.png" width="440" alt="已完成">

<details><summary>查看完整场景截图</summary>

![浅色](images/im93.png)

![深色](images/im95.png)

</details>

### 报错

红色点，保留错误摘要和展开详情。 局部聚焦左侧状态；右侧操作见完整原图。

真实组件 · 示例数据

**浅色**

<img src="images/im102.png" width="440" alt="报错">

**深色**

<img src="images/im104.png" width="440" alt="报错">

<details><summary>查看完整场景截图</summary>

![浅色](images/im103.png)

![深色](images/im105.png)

</details>

### 已取消

中性灰点，保留原详情与打开任务。 局部聚焦左侧状态；右侧操作见完整原图。

真实组件 · 示例数据

**浅色**

<img src="images/im106.png" width="440" alt="已取消">

**深色**

<img src="images/im107.png" width="440" alt="已取消">

<details><summary>查看完整场景截图</summary>

![浅色](images/im103.png)

![深色](images/im105.png)

</details>

