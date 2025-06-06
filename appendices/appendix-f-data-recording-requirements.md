## 附录F （规范性） 数据记录要求

### F.1 技术要求

#### F.1.1 总体要求

组合驾驶辅助数据记录系统分为I型系统和II型系统。

M₁类和N₁类车辆配备的组合驾驶辅助数据记录系统应为I型或II型系统，M₂、M₃、N₂和N₃车辆配备的组合驾驶辅助数据记录系统应为II型系统，相关要求如下：

> —— I型系统应满足本文件F.1.2、F.1.4至F.1.9的要求；

> —— II型系统应满足本文件F.1.3至F.1.9的要求。

#### F.1.2 I型系统数据记录要求

##### F.1.2.1 一般要求

**F.1.2.1.1** 当组合驾驶辅助系统激活期间，I型系统应至少记录如下事件数据：

> a) 时间段事件：当发生符合F.1.2.2.1要求的碰撞事件或符合F.1.2.3.1要求的有碰撞风险事件时，组合驾驶辅助数据记录系统应记录符合F.1.4.2要求的数据元素；

> b) 时间戳事件：当组合驾驶辅助系统进入激活状态时、退出时、发出HOR提示信号时、取消HOR提示或警告信号、发出EOR提示信号时、取消EOR提示或警告信号、发出DCA时、开始执行RMF时、发生组合驾驶辅助系统严重失效、车辆严重失效和用户操纵组合驾驶辅助系统退出装置时，组合驾驶辅助数据记录系统应记录符合表F.1要求的数据元素。

**F.1.2.1.2** 当前的时间段事件数据记录正在进行时，若在此期间发生时间段事件，可不完整记录后续发生的时间段事件相关数据，但应保证至少按照表F.1的要求记录后续发生的时间段事件的相关数据。

**F.1.2.1.3** 由于失效导致数据不可获取时，组合驾驶辅助数据记录系统可不完全记录时间戳事件和时间段事件数据。车辆制造商应提供相关文档进行说明。

##### F.1.2.2 碰撞事件

###### F.1.2.2.1 触发条件

当车辆符合GB 39732—2020中4.1.1的要求时，该事件应被记录。

###### F.1.2.2.2 事件起点和终点

碰撞事件起点和终点应符合如下要求：

> a) 事件起点：碰撞事件起点应符合GB 39732—2020中4.1.3的要求；

> b) 事件终点：碰撞事件终点应符合GB 39732—2020中4.1.4的要求。

###### F.1.2.2.3 事件记录起点和终点

碰撞事件记录起点和终点应至少符合如下要求：

> a) 事件记录起点：事件起点前15 s或组合驾驶辅助系统激活时刻，两者取较晚时刻；

> b) 事件记录终点：事件起点后5 s、组合驾驶辅助系统退出时刻或事件终点，三者取较早时刻。

###### F.1.2.2.4 事件锁定条件

碰撞事件锁定条件应至少符合GB 39732—2020中4.1.2的要求。

**注：** 行人保护装置展开可不定义为锁定事件。

##### F.1.2.3 有碰撞风险事件

###### F.1.2.3.1 触发条件

组合驾驶辅助数据记录系统应至少将以下两种方式之一作为有碰撞风险事件的触发条件：

> —— 当组合驾驶辅助系统请求的纵向减速度大于5 m/s²时；

> —— 当符合GB 轻型汽车自动紧急制动系统技术要求及试验方法或GB 重型汽车自动紧急制动系统技术要求及试验方法的AEBS启动紧急制动时。

> **注：** 允许组合驾驶辅助数据记录系统增加其他的条件作为有碰撞风险事件的触发条件，例如更低的请求的纵向减速度。

###### F.1.2.3.2 事件起点和终点

当有碰撞风险事件的触发条件为组合驾驶辅助系统请求的纵向减速度大于5 m/s²时，则有碰撞风险事件起点和终点应符合如下要求：

> a) 事件起点：组合驾驶辅助系统请求的纵向减速度大于5 m/s²的时刻；

> b) 事件终点：本次事件起点后组合驾驶辅助系统请求的纵向减速度不大于5 m/s²的时刻。

当有碰撞风险事件的触发条件为GB 轻型汽车自动紧急制动系统技术要求及试验方法或GB 重型汽车自动紧急制动系统技术要求及试验方法的AEB启动紧急制动时，该有碰撞风险事件起点和终点应符合如下要求：

> a) 事件起点：车辆AEBS启动紧急制动的时刻；

> b) 事件终点：车辆AEBS结束紧急制动的时刻。

###### F.1.2.3.3 事件记录起点和终点

有碰撞风险事件记录起点和终点应至少符合如下要求：

> a) 事件记录起点：事件起点前15 s或组合驾驶辅助系统激活时刻，两者取较晚时刻；

> b) 事件记录终点：事件起点后5 s、组合驾驶辅助系统退出时刻或事件终点，三者取较早时刻。

#### F.1.3 II型系统数据记录要求

在组合驾驶辅助系统激活期间，II型系统应至少记录如下数据：

> a) 在实时记录起点时刻记录符合表F.1要求的数据元素；

> b) 实时连续记录符合表F.2至表F.5要求的数据元素；

> c) 时间戳事件：当组合驾驶辅助系统进入激活状态时、退出时、发出HOR提示信号时、取消HOR提示或警告信号、发出EOR提示信号时、取消EOR提示或警告信号、发出DCA时、开始执行RMF时、发生组合驾驶辅助系统严重失效、车辆严重失效和用户操纵组合驾驶辅助系统退出装置时，组合驾驶辅助数据记录系统应记录符合表F.1要求的数据元素。

> **注：** 实时记录起点时刻指组合驾驶辅助系统激活时刻。

由于失效导致数据不可获取时，组合驾驶辅助数据记录系统可不完全记录时间戳事件和时间段事件数据。车辆制造商应提供相关文档进行说明。

#### F.1.4 数据元素要求

##### F.1.4.1 数据元素分级

组合驾驶辅助数据记录系统记录的数据元素应按照如下要求分为两级：

> —— A级数据元素：配备组合驾驶辅助数据记录系统的车辆应记录的数据元素；

> —— B级数据元素：对于车辆状态及动态信息，B级数据元素指配备获取相关数据元素的传感器时则应记录的数据元素；对于组合驾驶辅助系统运行信息，B级数据元素相关信号处于被组合驾驶辅助系统调用时应记录的数据元素。

##### F.1.4.2 数据元素记录要求

**F.1.4.2.1** 组合驾驶辅助数据记录系统应记录符合表F.1至表F.5中要求的数据元素。

<div align="center">
  <strong>表F.1 车辆及组合驾驶辅助数据记录系统基本信息</strong>

<table>
<thead>
  <tr>
    <th align="center">序号</th>
    <th align="center">数据名称</th>
    <th align="center">分级</th>
    <th align="center">最小记录频率</th>
    <th align="center">单位</th>
    <th align="center">最小记录数据能力范围</th>
    <th align="center">最低记录分辨率</th>
    <th align="center">最低记录准确度</th>
    <th align="center">数据说明</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">1</td>
    <td align="center">车辆识别代号(VIN)</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">车辆识别代号格式应符合GB 16735的要求</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">实现组合驾驶辅助数据记录系统功能的硬件型号</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">实现组合驾驶辅助数据记录系统功能的硬件序列号</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">4</td>
    <td align="center">组合驾驶辅助系统软件版本号</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">一如果具备软件识别功能，可记录组合驾驶辅助系统软件识别码</td>
  </tr>
  <tr>
    <td align="center">5</td>
    <td align="center">组合驾驶辅助数据记录系统软件版本号</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">一如果具备软件识别功能，可记录组合驾驶辅助数据记录系统软件识别码</td>
  </tr>
  <tr>
    <td align="center">6</td>
    <td align="center">事件类型编码</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="left">7：锁定碰撞<br/>8：有碰撞风险<br/>10：非锁定碰撞<br/>20：组合驾驶辅助系统激活<br/>21：组合驾驶辅助系统主动退出<br/>22：用户操纵组合驾驶辅助系统退出<br/>23：组合驾驶辅助系统发出HOR提示信号<br/>24：组合驾驶辅助系统取消HOR提示或警告信号<br/>25：组合驾驶辅助系统发出EOR提示信号<br/>26：组合驾驶辅助系统取消EOR提示或警告信号<br/>27：发出DCA<br/>28：开始执行RMF<br/>29：组合驾驶辅助系统严重失效<br/>30：车辆严重失效</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">7</td>
    <td align="center">时间（年）</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">年</td>
    <td align="center">2023~2253</td>
    <td align="center">1</td>
    <td align="center" rowspan='6'>相对于协调世界时应用UTC0时间（UTC），不应存在秒级误差</td>
    <td align="center" rowspan='6'>应为UTC0时间</td>
  </tr>
  <tr>
    <td align="center">8</td>
    <td align="center">时间（月）</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">月</td>
    <td align="center">1~12</td>
    <td align="center">1</td>
  </tr>
  <tr>
    <td align="center">9</td>
    <td align="center">时间（日）</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">日</td>
    <td align="center">1~31</td>
    <td align="center">1</td>
  </tr>
  <tr>
    <td align="center">10</td>
    <td align="center">时间（时）</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">时</td>
    <td align="center">0~23</td>
    <td align="center">1</td>
  </tr>
  <tr>
    <td align="center">11</td>
    <td align="center">时间（分）</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">分</td>
    <td align="center">0~59</td>
    <td align="center">1</td>
  </tr>
  <tr>
    <td align="center">12</td>
    <td align="center">时间（秒）</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">秒</td>
    <td align="center">0~60</td>
    <td align="center">1</td>
  </tr>
  <tr>
    <td align="center">13</td>
    <td align="center">累计行驶里程</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">km</td>
    <td align="center">0~600000</td>
    <td align="center">1</td>
    <td align="center">±1</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">14</td>
    <td align="center">连续条次时间段基准性的事件类型</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="left">7：非锁定碰撞<br/>8：有碰撞风险<br/>10：锁定碰撞</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">仅针对连续时间段基准性</td>
  </tr>
  <tr>
    <td align="center">15</td>
    <td align="center">连续多次时间段事件的事件起点时刻(年)</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">年</td>
    <td align="center">2023~2253</td>
    <td align="center">1</td>
    <td align="center" rowspan='6'>相对于协调世界时(UTC)，不应存在秒级误差</td>
    <td align="center" rowspan='6'>仅针对连续时间段事件性且应为UTC时间</td>
  </tr>
  <tr>
    <td align="center">16</td>
    <td align="center">连续多次时间段事件的事件起点时刻(月)</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">月</td>
    <td align="center">1~12</td>
    <td align="center">1</td>
  </tr>
  <tr>
    <td align="center">17</td>
    <td align="center">连续多次时间段事件的事件起点时刻(日)</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">日</td>
    <td align="center">1~31</td>
    <td align="center">1</td>
  </tr>
  <tr>
    <td align="center">18</td>
    <td align="center">连续多次时间段事件的事件起点时刻(时)</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">时</td>
    <td align="center">0~23</td>
    <td align="center">1</td>
  </tr>
  <tr>
    <td align="center">19</td>
    <td align="center">连续多次时间段事件的事件起点时刻(分)</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">分</td>
    <td align="center">0~59</td>
    <td align="center">1</td>
  </tr>
  <tr>
    <td align="center">20</td>
    <td align="center">连续多次时间段事件的事件起点时刻(秒)</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">秒</td>
    <td align="center">0~60</td>
    <td align="center">1</td>
  </tr>
  <tr>
    <td align="center">21</td>
    <td align="center">事件记录完整标志</td>
    <td align="center">A</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="left">1：完整<br/>0：不完整</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="left">完整的事件数据集是否成功记录并存储在组合驾驶辅助数据记录系统中的状态，仅适用于时间段事件</td>
  </tr>
</tbody>
</table>

<p align="left" style="margin-top: 10px;">
表F.1中的序号1至序号5数据元素应保证在数据读取时能够被正确读取。表F.1中序号6至序号13数据元素应至少在事件起点或实时记录起点时刻记录。表F.1中序号14至序号21数据元素应至少在事件记录终点时刻记录。<br/>
当能够单独记录连续多次时间段事件时，表F.1序号14至序号20数据元素可不记录。
</p>

</div>

<div align="center">
  <strong>表F.2 车辆状态及动态信息</strong>

<table>
<thead>
  <tr>
    <th align="center">序号</th>
    <th align="center">数据名称</th>
    <th align="center">分级</th>
    <th align="center">最小记录频率</th>
    <th align="center">单位</th>
    <th align="center">最小记录数据能力范围</th>
    <th align="center">最低记录分辨率</th>
    <th align="center">最低准确度</th>
    <th align="center">数据说明</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">1</td>
    <td align="center">车辆速度</td>
    <td align="center">A</td>
    <td align="center">10 Hz</td>
    <td align="center">km/h</td>
    <td align="center">0~240</td>
    <td align="center">1</td>
    <td align="center">±10%</td>
    <td align="center">非仪表显示车速，应与车辆运行实际速度保持一致</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">车辆横向加速度</td>
    <td align="center">A</td>
    <td align="center">10 Hz</td>
    <td align="center">m/s²</td>
    <td align="center">-20~20</td>
    <td align="center">1</td>
    <td align="center">传感器探测范围的±10%</td>
    <td align="center">当驾驶员坐在车内面向车辆行驶方向，从驾驶员角度看从左向右为正方向</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">车辆纵向加速度</td>
    <td align="center">A</td>
    <td align="center">10 Hz</td>
    <td align="center">m/s²</td>
    <td align="center">-20~20</td>
    <td align="center">1</td>
    <td align="center">传感器探测范围的±10%</td>
    <td align="center">车辆向前行驶方向为正方向</td>
  </tr>
  <tr>
    <td align="center">4</td>
    <td align="center">车辆横摆角速度<sup>a</sup></td>
    <td align="center">A</td>
    <td align="center">2 Hz</td>
    <td align="center">°/s</td>
    <td align="center">-75~75</td>
    <td align="center">0.1</td>
    <td align="center">传感器探测范围的±10%</td>
    <td align="center">车辆相对Z轴的角度变化，顺时针为正方向</td>
  </tr>
  <tr>
    <td align="center">5</td>
    <td align="center">车辆侧倾角速度<sup>a</sup></td>
    <td align="center">B</td>
    <td align="center">2 Hz</td>
    <td align="center">°/s</td>
    <td align="center">-75~75</td>
    <td align="center">1</td>
    <td align="center">传感器探测范围的±10%</td>
    <td align="center">车辆相对X轴的角度变化，逆时针为正方向</td>
  </tr>
  <tr>
    <td align="center">6</td>
    <td align="center">航向角</td>
    <td align="center">B</td>
    <td align="center">2 Hz</td>
    <td align="center">°</td>
    <td align="center">-180~180</td>
    <td align="center">1</td>
    <td align="center">±5</td>
    <td align="center">正北方向为0°，顺时针方向为正方向</td>
  </tr>
  <tr>
    <td align="center">7</td>
    <td align="center">转向盘角度</td>
    <td align="center">A</td>
    <td align="center">2 Hz</td>
    <td align="center">°</td>
    <td align="center">-200~200</td>
    <td align="center">5</td>
    <td align="center">全部范围时的±5%</td>
    <td align="center">转向盘逆时针方向转动为正方向。</td>
  </tr>
</tbody>
</table>

<p align="left" style="margin-top: 10px;">
<sup>a</sup>用于标识车辆横摆角速度和车辆侧倾角速度方向的车辆坐标系应符合GB 39732中对于车辆坐标系的定义。
</p>

</div>

<div align="center">
  <strong>表F.3 组合驾驶辅助系统运行信息</strong>

<table>
<thead>
  <tr>
    <th align="center">序号</th>
    <th align="center">数据名称</th>
    <th align="center">分级</th>
    <th align="center">最小记录频率</th>
    <th align="center">单位</th>
    <th align="center">最小记录数据能力范围</th>
    <th align="center">最低记录分辨率</th>
    <th align="center">最低准确度</th>
    <th align="center">数据说明</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">1</td>
    <td align="center">组合驾驶辅助系统请求的横向加速度</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">m/s²</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">0.5</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">组合驾驶辅助系统请求的转向盘转向角</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">°</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">1</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">组合驾驶辅助系统请求的转向曲率</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">1/m</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">0.001</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">4</td>
    <td align="center">组合驾驶辅助系统请求的前轮转角</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">°</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">0.1</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">5</td>
    <td align="center">组合驾驶辅助系统请求的转向小齿轮转向角</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">°</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">0.005</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">6</td>
    <td align="center">组合驾驶辅助系统请求的转向盘转向力矩</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">Nm</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">0.1</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">7</td>
    <td align="center">组合驾驶辅助系统请求的转向盘转向角速率</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">°/s</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">10</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">8</td>
    <td align="center">组合驾驶辅助系统请求的车速</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">km/h</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">1</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">9</td>
    <td align="center">组合驾驶辅助系统请求的纵向加速度</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">m/s²</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">0.5</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">10</td>
    <td align="center">组合驾驶辅助系统请求的加速踏板开度比例</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">%</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">1</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">11</td>
    <td align="center">组合驾驶辅助系统请求的制车踏板开度比例</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">%</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">1</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">12</td>
    <td align="center">组合驾驶辅助系统请求的驱动转矩</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">Nm</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">1</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">13</td>
    <td align="center">组合驾驶辅助系统请求的驱动转速</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">rpm</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">100</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">14</td>
    <td align="center">组合驾驶辅助系统请求的轮端扭矩</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">Nm</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">1</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">15</td>
    <td align="center">组合驾驶辅助系统请求的制动主缸压力</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">MPa</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">1</td>
    <td align="center">由企业自定义，应与组合驾驶辅助系统实际能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">16</td>
    <td align="center">组合驾驶辅助系统请求的挡位</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">不适用</td>
    <td align="center">1：P挡<br/>2：R挡<br/>3：N挡<br/>4：D挡</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">17</td>
    <td align="center">组合驾驶辅助系统请求的自适应前照明系统状态</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">不适用</td>
    <td align="center">1：开启自适应照明系统<br/>0：关闭自适应照明系统</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">18</td>
    <td align="center">组合驾驶辅助系统请求的近灯光状态</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">不适用</td>
    <td align="center">1：开启<br/>0：关闭</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">19</td>
    <td align="center">组合驾驶辅助系统请求的远光灯状态</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">不适用</td>
    <td align="center">1：开启<br/>0：关闭</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">20</td>
    <td align="center">组合驾驶辅助系统请求的危险警告信号状态</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">不适用</td>
    <td align="center">1：开启<br/>0：关闭</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">21</td>
    <td align="center">组合驾驶辅助系统请求的制动灯状态</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">不适用</td>
    <td align="center">1：开启<br/>0：关闭</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">22</td>
    <td align="center">组合驾驶辅助系统请求的左转向信号灯状态</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">不适用</td>
    <td align="center">1：开启<br/>0：关闭</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">23</td>
    <td align="center">组合驾驶辅助系统请求的右转向信号灯状态</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">不适用</td>
    <td align="center">1：开启<br/>0：关闭</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">24</td>
    <td align="center">组合驾驶辅助系统请求的车辆雨刮状态</td>
    <td align="center">B</td>
    <td align="center">4 Hz</td>
    <td align="center">不适用</td>
    <td align="center">1：开启<br/>0：关闭</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">设计运行条件若包含雨天时，应记录该数据</td>
  </tr>

</tbody>
</table>

<p align="left" style="margin-top: 10px;">
1. 组合驾驶辅助数据记录系统记录序号1到序号7任一数据元素、序号8至序号15任一数据元素即视为满足本文件要求。</br>
2. 组合驾驶辅助数据记录系统应按表F.3中的要求记录序号16至序号24数据元素。
</p>

</div>

<div align="center">
  <strong>表F.4 行车环境信息</strong>

<table>
<thead>
  <tr>
    <th align="center">序号</th>
    <th align="center">数据名称</th>
    <th align="center">分级</th>
    <th align="center">最小记录频率</th>
    <th align="center">单位</th>
    <th align="center">最小记录数据能力范围</th>
    <th align="center">最低记录分辨率</th>
    <th align="center">最低记录准确度</th>
    <th align="center">数据说明</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">1</td>
    <td align="center">感知目标物ID</td>
    <td align="center">A</td>
    <td align="center">10 Hz</td>
    <td align="center">不适用</td>
    <td align="center">由企业自定义</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">编号方式由企业自定义</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">感知目标物类型</td>
    <td align="center">A</td>
    <td align="center">10 Hz</td>
    <td align="center">不适用</td>
    <td align="center">由企业自定义，应与车辆实际感知能力相符</td>
    <td align="center">不适用</td>
    <td align="center">应与车辆实际感知能力相符</td>
    <td align="center">记录的目标物类型是自动驾驶系统识别的最大概率目标物类型</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">感知目标物相对位置(X向)</td>
    <td align="center">A</td>
    <td align="center">10 Hz</td>
    <td align="center">m</td>
    <td align="center">由企业自定义，应与车辆实际感知能力相符</td>
    <td align="center">0.5</td>
    <td align="center">应与车辆实际感知能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">4</td>
    <td align="center">感知目标物相对位置(Y向)</td>
    <td align="center">A</td>
    <td align="center">10 Hz</td>
    <td align="center">m</td>
    <td align="center">由企业自定义，应与车辆实际感知能力相符</td>
    <td align="center">0.5</td>
    <td align="center">应与车辆实际感知能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">5</td>
    <td align="center">感知目标物相对速度(X向)</td>
    <td align="center">A</td>
    <td align="center">10 Hz</td>
    <td align="center">km/h</td>
    <td align="center">由企业自定义，应与车辆实际感知能力相符</td>
    <td align="center">1</td>
    <td align="center">应与车辆实际感知能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">6</td>
    <td align="center">感知目标物相对速度(Y向)</td>
    <td align="center">A</td>
    <td align="center">10 Hz</td>
    <td align="center">km/h</td>
    <td align="center">由企业自定义，应与车辆实际感知能力相符</td>
    <td align="center">1</td>
    <td align="center">应与车辆实际感知能力相符</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">7</td>
    <td align="center">外部图像<sup>a</sup></td>
    <td align="center">A</td>
    <td align="center">4 Hz</td>
    <td align="center">不适用</td>
    <td align="left" rowspan='2'>组合驾驶辅助数据记录系统记录的外部图像或视频数据应至少满足以下任一要求：</br>——若仅记录车辆前向图像或视频，水平视场角应不低于100°,垂直视场角应不低于35°，有效像素不低于90万；</br>——若同时记录车辆前向、左侧、右侧和后向四路图像或视频，水平视场角应能覆盖360°，单路有效像素应不低于28万</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">应具有百毫秒级时间戳信息，且应能被正确解析</td>
  </tr>
  <tr>
    <td align="center">8</td>
    <td align="center">外部视频</td>
    <td align="center">A</td>
    <td align="center">4 fps</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">不适用</td>
    <td align="center">应具有百叠秒级时间戳信息，且应能被正确解析</td>
  </tr>
</tbody>
</table>

<p align="left" style="margin-top: 10px;">
组合驾驶辅助数据记录系统应至少具备记录8个目标物的能力，若实际目标物小于8，组合驾驶辅助系统记录实际目标物的数量即可。每个目标物的记录信息均应包含符合本表要求的序号1~序号6的数据元素。</br>
<strong>注：</strong>本表中相对位置和相对速度的测量均基于同一坐标系：将车辆后轴重点作为坐标系原点，X轴平行于车辆的纵向对称平面并指向车辆前方，Y轴垂直于车辆的纵向对称平面并指向车辆左侧。</br><strong>注：</strong>若组合驾驶辅助系统采用网络模型无法生成感知目标物信息，可不记录本表中序号1-6数据元素。</br>
<sup>a</sup>外部图像或外部视频应至少记录一种。
</p>

</div>

<div align="center">
  <strong>表F.5 驾驶员操作及状态信息</strong>

<table>
<thead>
  <tr>
    <th align="center">序号</th>
    <th align="center">数据名称</th>
    <th align="center">分级</th>
    <th align="center">最小记录频率</th>
    <th align="center">单位</th>
    <th align="center">最小记录数据能力范围</th>
    <th align="center">最低记录分辨率</th>
    <th align="center">最低记录准确度</th>
    <th align="center">数据说明</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">1</td>
    <td align="center">驾驶员是否系安全带</td>
    <td align="center">A</td>
    <td align="center">2 Hz</td>
    <td align="center">不适用</td>
    <td align="center">0：未系安全带<br/>1：系安全带</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">驾驶员是否在驾驶位置</td>
    <td align="center">A</td>
    <td align="center">2 Hz</td>
    <td align="center">不适用</td>
    <td align="center">0：否<br/>1：是</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">驾驶员是否手部脱离</td>
    <td align="center">A</td>
    <td align="center">2 Hz</td>
    <td align="center">不适用</td>
    <td align="center">0：否<br/>1：是</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">4</td>
    <td align="center">驾驶员是否视线脱离</td>
    <td align="center">A</td>
    <td align="center">2 Hz</td>
    <td align="center">不适用</td>
    <td align="center">0：否<br/>1：是</td>
    <td align="center">不适用</td>
    <td align="center">不应有误差</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">5</td>
    <td align="center">加速踏板开度</td>
    <td align="center">A</td>
    <td align="center">2 Hz</td>
    <td align="center">%</td>
    <td align="center">0~100</td>
    <td align="center">1</td>
    <td align="center">全部范围的±10%</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">6</td>
    <td align="center">刹车踏板开度<sup>a, b</sup></td>
    <td align="center">A</td>
    <td align="center">2 Hz</td>
    <td align="center">%</td>
    <td align="center">0~100</td>
    <td align="center">1</td>
    <td align="center">全部范围的±10%</td>
    <td align="left">如不具备记录踏板开度的条件，应记录刹车踏板状态，记录的状态应至少包含：<br/>0：否<br/>1：是</td>
  </tr>
  <tr>
    <td align="center">7</td>
    <td align="center">输入转向扭矩<sup>c</sup></td>
    <td align="center">A</td>
    <td align="center">2 Hz</td>
    <td align="center">Nm</td>
    <td align="center">-10~10</td>
    <td align="center">0.1</td>
    <td align="center">±1</td>
    <td align="center">—</td>
  </tr>
  <tr>
    <td align="center">8</td>
    <td align="center">系统激活后用户设置巡航车速</td>
    <td align="center">A</td>
    <td align="center">2 Hz</td>
    <td align="center">km/h</td>
    <td align="center">0~240</td>
    <td align="center">1</td>
    <td align="center">±10%</td>
    <td align="center">—</td>
  </tr>
</tbody>
</table>

<p align="left" style="margin-top: 10px;">
<sup>a</sup> 如果已经记录了刹车踏板开度,可不记录刹车踏板状态。</br>
<sup>b</sup> 刹车踏板有效开度上限若小于100,可将刹车踏板有效开度上限作为最小记录数据能力范围的上限值。</br>
<sup>c</sup> 输入转向扭矩逆时针方向为正方向。
</p>

</div>

**F.1.4.2.2** 表F.1至表F.5中的数据元素应能时间同步。所有的数据都应有时间戳，且所有的时间戳应来自于同一时间源。

#### F.1.5 数据存储要求

##### F.1.5.1 存储介质

组合驾驶辅助数据记录系统记录的数据应存储在车端非易失性存储器中。

##### F.1.5.2 存储能力

组合驾驶辅助数据记录系统应符合如下要求：

> a) I型系统能存储的碰撞事件和碰撞风险事件次数总体不应少于5次，且能存储的时间戳事件次数不应少于2500次。

> b) II型系统能存储的连续数据不应少于8 h，且能存储的时间戳事件次数不应少于2500次。

> **注：** 当车辆组合驾驶数据记录系统和自动驾驶数据记录系统设计为同一系统时，该系统的存储能力满足组合驾驶辅助数据记录系统和自动驾驶数据记录系统两者中存储能力要求较高者即可，不需要达到两者存储能力要求的总和。

##### F.1.5.3 存储覆盖机制

###### F.1.5.3.1 I型系统

I型系统存储区域已满时，应满足如下存储覆盖要求：

> a) 时间段事件数据和时间戳事件数据不应互相覆盖；

> b) 对于时间段事件，碰撞事件数据不应被有碰撞风险事件数据覆盖；

> c) 满足锁定条件的碰撞事件数据，不应被后续事件的数据覆盖；

> d) 其他情况应按照时间顺序依次覆盖；

> e) 当I型系统存储区域已满且存储的时间段数据均为锁定事件数据时，在将全部锁定事件数据在平台或者服务器实现安全存储的情况下，组合驾驶辅助数据记录系统的锁定时间段事件数据可被覆盖。

> **注：** 当车辆组合驾驶数据记录系统和自动驾驶数据记录系统设计为同一系统时，该系统的存储覆盖机制在遵循上述存储覆盖要求基础上，组合驾驶辅助数据和自动驾驶数据可按时间顺序依次覆盖。

###### F.1.5.3.2 II型系统

II型系统存储区域已满时，应满足如下存储覆盖要求：

> a) 实时连续记录的数据与时间戳事件数据不应互相覆盖；

> b) 其他情况应按照时间顺序依次覆盖。

###### F.1.5.3.3 多个组合驾驶辅助数据记录系统

如果车辆同时具备I型和II型组合驾驶辅助数据记录系统，I型系统和II型系统记录的数据不应互相覆盖。

##### F.1.5.4 断电存储

组合驾驶辅助系统激活期间，如碰撞事件导致组合驾驶辅助数据记录系统无法被正常供电，组合驾驶辅助数据记录系统应至少记录事件记录起点至事件起点的数据，视频和图像数据除外。

无法被正常供电：具备冗余供电方式的组合驾驶辅助数据记录系统无法继续由非冗余供电方式供电。

#### F.1.6 数据读取要求

##### F.1.6.1 总体要求

组合驾驶辅助数据记录系统记录的数据应能被读取并正确解析，包括整车和部件级别的读取。

整车级别的数据读取方式应至少支持下列方式之一：

> —— 符合GB 39732-2020 4.4.3.1的读取方式，其数据元素排列应符合F.4；

> —— 符合GB 44497-2024 4.6.2至4.6.4的读取方式；

#### F.1.7 信息安全要求

**F.1.7.1** 组合驾驶辅助数据记录系统应具备安全启动功能，应保护组合驾驶辅助数据记录系统的可信根、引导加载程序、系统固件不被篡改，或被篡改后无法正常启动。

**F.1.7.2** 组合驾驶辅助数据记录系统应采取有效的安全防御机制保护存储的数据。若发生篡改和非授权的删除，则组合驾驶辅助数据记录系统应至少能在读取时通过技术手段识别并记录。

#### F.1.8 耐撞性能要求

按照F.3.3进行试验，组合驾驶辅助数据记录系统记录的数据至少应与试验前的数据保持一致。

#### F.1.9 环境评价性要求

##### F.1.9.1 功能状态定义

组合驾驶辅助数据记录系统记录的数据应能够被正确读取、解析且与试验前数据保持一致。

##### F.1.9.2 电气性能

###### F.1.9.2.1 直流供电电压

实现组合驾驶辅助数据记录系统功能的控制器直流供电电压范围见表F.6，按照F.3.6.1.1进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.2.2 过电压

**F.1.9.2.2.1 （T<sub>max</sub>-20℃）条件**

按照F.3.6.1.2.1进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

**F.1.9.2.2.2 室温条件下**

按照F.3.6.1.2.2进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.2.3 叠加交流电压

按照F.3.6.1.3进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.2.4 供电电压缓降和缓升

按照F.3.6.1.4进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.2.5 供电电压瞬态变化

**F.1.9.2.5.1 电压瞬时下降**

按照F.3.6.1.5.1进行试验，试验后，产品功能状态应满足F.1.9.1得要求。

**F.1.9.2.5.2 对电压骤降的复位性能**

按照F.3.6.1.5.2进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

<div align="center">
  <strong>表F.6 直流供电电压范围</strong>

<p align="right" style="margin-top: 10px;">
单位为伏
</p>

<table>
<thead>
  <tr>
    <th align="center">标称电压 U<sub>N</sub></th>
    <th align="center">最小电压 U<sub>min</sub></th>
    <th align="center">最大电压 U<sub>Smax</sub></th>
    <th align="center">试验电压 U<sub>A</sub></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">12</td>
    <td align="center">9</td>
    <td align="center">16</td>
    <td align="center">14±0.2</td>
  </tr>
  <tr>
    <td align="center">24</td>
    <td align="center">16</td>
    <td align="center">32</td>
    <td align="center">28±0.2</td>
  </tr>
</tbody>
</table>

</div>

**F.1.9.2.5.3 启动特性**

按照F.3.6.1.5.3进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

> **注：** 该要求不适用于仅用于纯电动汽车的组合驾驶辅助数据记录系统。

**F.1.9.2.5.4 抛负载**

按照F.3.6.1.5.4进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

> **注：** 该要求不适用于仅用于纯电动汽车的组合驾驶辅助数据记录系统。

 ###### F.1.9.2.6 反向电压

按照F.3.6.1.6进行试验，试验后，需要进行内部检查，产品内部元器件应无损伤，产品功能状态应满足F.1.9.1的要求。

> **注：** 该要求不适用于带有钳位二极管而没有外部反极性保护的组合驾驶辅助数据记录系统。

###### F.1.9.2.7 参考接地和供电偏移

对于多点接地的组合驾驶辅助数据记录系统，按照F.3.6.1.7进行试验，试验后,产品功能状态应满足F.1.9.1的要求。

###### F.1.9.2.8 开路

**F.1.9.2.8.1 单线开路**

按照F.3.6.1.8.1进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

**F.1.9.2.8.2 多线开路**

按照F.3.6.1.8.2进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.2.9 短路保护

按照F.3.6.1.9进行试验，试验后，产品功能状态满足应F.1.9.1的要求。

###### F.1.9.2.10 绝缘电阻

按照F.3.6.1.10进行试验，组合驾驶辅助数据记录系统的绝缘电阻应大于10 MΩ。试验后，产品功能状态应满足F.1.9.1的要求。

##### F.1.9.3 防尘防水性能

组合驾驶辅助数据记录系统防护等级应符合表F.7的规定，按照F.3.6.2进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

<div align="center">
  <strong>表F.7 防水防尘等级</strong>

<table>
<thead>
  <tr>
    <th align="center">安装位置</th>
    <th align="center">防水防尘等级</th>
    <th align="center">描述</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">发动机舱</td>
    <td align="center">IP5K6</td>
    <td align="center">粉尘防护，强高度喷水</td>
  </tr>
  <tr>
    <td align="center">车辆内部</td>
    <td align="center">IP5K1</td>
    <td align="center">粉尘防护，垂直滴水</td>
  </tr>
  <tr>
    <td align="center">行李箱</td>
    <td align="center">IP5K1</td>
    <td align="center">粉尘防护，垂直滴水</td>
  </tr>
</tbody>
</table>

</div>

##### F.1.9.4 环境耐候性

###### F.1.9.4.1 温湿度范围

组合驾驶辅助数据记录系统的工作环境温度应符合GB/T 28046.4—2013表1中的相应要求。

###### F.1.9.4.2 低温贮存

按照F.3.6.3.1进行试验，试验后，产品不允许损坏，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.4.3 低温工作

按照F.3.6.3.2进行试验，试验后，产品不允许损坏，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.4.4 高温贮存

按照F.3.6.3.3进行试验，试验后，产品不允许损坏，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.4.5 高温工作

按照F.3.6.3.4进行试验，试验后，产品不允许损坏，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.4.6 温度梯度

按照F.3.6.3.5进行试验，试验后，产品不允许损坏，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.4.7 规定转换时间的温度快速变化

按照F.3.6.3.6进行试验，试验后，产品不允许损坏，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.4.8 规定变化率的温度循环

按照F.3.6.3.7进行试验，试验后，产品不允许损坏，功能状态应满足F.1.9.1的要求。

###### F.1.9.4.9 湿热循环

按照F.3.6.3.8进行试验，试验后，产品不允许损坏，功能状态应满足F.1.9.1的要求。

###### F.1.9.4.10 稳态湿热

按照F.3.6.3.9进行试验，试验后，产品不允许损坏，功能状态应满足F.1.9.1的要求。

###### F.1.9.4.11 太阳光辐射

安装在乘客舱内太阳直射处的组合驾驶辅助数据记录系统，按照F.3.6.3.10进行试验，试验后，表面不应有脱落、龟裂、气泡等现象。

安装在非太阳直射处的组合驾驶辅助数据记录系统不作要求。

##### F.1.9.5 机械性能

###### F.1.9.5.1 机械振动

按照F.3.6.4.1进行试验，试验后，产品不允许损坏，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.5.2 机械冲击

按照F.3.6.4.2进行试验，试验后，产品不允许损坏，产品功能状态应满足F.1.9.1的要求。

##### F.1.9.6 化学负荷

按照F.3.6.5进行试验，试验后，产品不允许损坏，标志和标签应保持清晰可见，产品功能状态应满足F.1.9.1的要求。

##### F.1.9.7 电磁兼容性能

###### F.1.9.7.1 对静电放电产生的电骚扰抗扰

**F.1.9.7.1.1 电子模块不通电**

按照F.3.6.6.1.1进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

**F.1.9.7.1.2 电子模块通电**

按照F.3.6.6.1.2进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.7.2 对由传导和耦合引起的电骚扰抗扰

**F.1.9.7.2.1 沿电源线的电瞬态传导抗扰**

按照F.3.6.6.2.1进行试验，抗扰试验等级和试验要求应符合表F.8的规定。

<div align="center">
  <strong>表F.8 沿电源线瞬态传导的抗扰性能</strong>

<table>
<thead>
  <tr>
    <th align="center">试验脉冲</th>
    <th align="center">抗扰试验等级</th>
    <th align="center">试验要求</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">1</td>
    <td align="center">III</td>
    <td align="center" rowspan="4">产品功能状态满足 F.1.9.1 的要求</td>
  </tr>
  <tr>
    <td align="center">2a</td>
    <td align="center">III</td>
  </tr>
  <tr>
    <td align="center">2b</td>
    <td align="center">III</td>
  </tr>
  <tr>
    <td align="center">3a/3b</td>
    <td align="center">III</td>
  </tr>
  <tr>
    <td colspan="3">注：抗扰试验等级定义见GB/T 21437.2—2021中的附录A。</td>
  </tr>
</tbody>
</table>

</div>

**F.1.9.7.2.2 除电源线外的导线通过容性和感性耦合的电瞬态抗扰**

按照F.3.6.6.2.2进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.7.3 对电磁辐射的抗扰

按照F.3.6.6.3进行试验，试验后，产品功能状态应满足F.1.9.1的要求。

###### F.1.9.7.4 无线电骚扰特性

按照F.3.6.6.4进行试验，试验后，组合驾驶辅助数据记录系统应满足GB 34660—2017中4.5和4.6的要求。

### F.2 试验条件

#### F.2.1 试验场地及试验环境要求

##### F.2.1.1 试验场地应满足以下条件：

> a) 试验场地具有良好的路面附着能力；

> b) 交通标志和标线清晰可见；

> c) 具备试验车辆组合驾驶辅助功能模式正常激活的必要数据和设施条件。

##### F.2.1.2 天气条件

试验车辆应在天气良好且光照正常的环境下进行试验。

#### F.2.2 试验设备及数据记录要求

##### F.2.2.1 试验数据记录内容及要求

试验过程应记录以下内容：

> a) 表F.1车辆及组合驾驶辅助数据记录系统基本信息；

> b) 表F.2车辆状态及动态信息；

> c) 表F.5驾驶员操作及状态信息。

##### F.2.2.2 信号转化要求

**F.2.2.2.1** 如果采用F.3.1.2.2或F.3.1.2.4试验方法进行试验，车辆制造商应提供与车辆连接的软件或硬件装置，可注入能够触发碰撞事件（包括锁定事件和非锁定事件）的信号。

**F.2.2.2.2** 车辆制造商应按本文件要求提供数据读取工具。

##### F.2.2.3 目标物

车辆目标、自行车和摩托车应为大批量生产的乘用车、两轮自行车和两轮普通摩托车，或表面特征参数能够代表上述车辆且适应传感器系统的柔性目标。其中，车辆目标速度控制准确度应为±2 km/h。

> **注：** 两轮普通摩托车指车辆纵向中心平面上装有两个车轮的普通摩托车，其尺寸为长小于等于2.5 m，宽小于等于1.0 m，高小于等于1.4 m。

#### F.2.3 试验车辆要求

试验车辆应满足以下要求：

> a) 组合驾驶辅助功能在测试场地内正常开启；

> b) 组合驾驶辅助数据记录系统应存满时间段事件和时间戳事件，时间段事件包含1次锁定事件；

> c) 具备便于人工激活和关闭组合驾驶辅助模式的操作方式；

> d) 系统状态及人机转换过程提示信息清晰可见。

### F.3 试验方法

#### F.3.1 触发试验

##### F.3.1.1 时间戳事件触发试验

###### F.3.1.1.1 试验方法

激活试验车辆的组合驾驶辅助系统，并使组合驾驶辅助系统稳定运行，进行如下操作后，试验终止：

> —— 使组合驾驶辅助系统进入激活状态、发出HOR提示信号、发出HOR警告信号、取消HOR提示信号、取消HOR警告信号、发出EOR提示信号、发出EOR警告信号时、取消EOR提示信号、取消EOR警告信号时、发出DCA时、执行RMF、主动退出、用户操纵组合驾驶辅助系统退出装置；

> —— 在试验车辆低速运行或者静止且组合驾驶辅助系统未退出的条件下，通过信号注入或者实车模式的方式模拟车辆和组合驾驶系统严重失效。

###### F.3.1.1.2 通过要求

试验后，按照F.1.6的要求读取组合驾驶辅助数据记录系统记录的时间戳事件数据，I型系统记录的事件应符合F.1.2.1.1 b）的要求，II型系统记录的时间应符合F.1.3 c) 的要求。

##### F.3.1.2 碰撞事件触发试验

###### F.3.1.2.1 碰撞事件触发条件试验

**F.3.1.2.1.1 试验准备**

试验前应提交材料说明以下内容：

> —— 碰撞注入信号的类型和具体含义；

> —— 碰撞注入信号传输至组合驾驶辅助数据记录系统的具体链路；

> —— 碰撞注入信号触发碰撞事件的逻辑。

**F.3.1.2.1.2 试验方法**

实现碰撞事件触发条件检测功能的控制器应按照GB 39732—2020中5.3.2进行试验。

**F.3.1.2.1.3 通过要求**

试验后，读取组合驾驶辅助数据记录系统记录的事件数据，组合驾驶辅助数据记录系统对于事件的触发应符合F.1.2.2.1的要求。

###### F.3.1.2.2 碰撞事件触发记录试验

**F.3.1.2.2.1 总体要求**

碰撞事件触发试验应选取F.3.1.2.2.2、F.3.1.2.2.3和F.3.1.2.2.4任意一种方法进行试验。

**F.3.1.2.2.2 对于具备信号注入条件的数据记录系统**

**F.3.1.2.2.2.1 试验准备**

试验前应提交材料说明以下内容：

> —— 碰撞注入信号的类型和具体含义；

> —— 碰撞注入信号传输至组合驾驶辅助数据记录系统的具体链路；

> —— 碰撞注入信号触发碰撞事件的逻辑。

> —— 若碰撞注入信号触发碰撞事件的逻辑符合GB 39732—2020中4.1.1章节描述的触发逻辑，应提交汽车事件数据记录系统测试报告证明；否则应按照GB 39732—2020中5.3.2进行试验，并提交测试报告。

**F.3.1.2.2.2.2 试验方法**

对于配备I型系统的试验车辆，激活组合驾驶辅助系统，并使组合驾驶辅助系统稳定运行，注入能触发碰撞事件的信号，待组合驾驶辅助数据记录系统完成本次事件记录后，试验终止。

**F.3.1.2.2.2.3 通过要求**

试验后，读取组合驾驶辅助数据记录系统记录的事件数据，组合驾驶辅助数据记录系统对于事件的触发应符合F.1.2.2.3的要求。

**F.3.1.2.2.3 对于不具备信号注入条件的数据记录系统**

**F.3.1.2.2.3.1 试验方法**

对于配备I型系统的试验车辆，激活组合驾驶辅助系统，并使组合驾驶辅助系统稳定运行，采用但不限以下三种方式之一进行试验，待组合驾驶辅助数据记录系统完成本次事件记录后，试验终止：

> —— 撞击车辆，使车辆达到GB 39732规定的触发阈值;

> —— 物理触发车辆的事件数据记录（EDR）系统，使车辆达到GB 39732规定的触发阈值;

> —— 对车辆EDR输入触发信号，使车辆达到GB 39732规定的触发阈值。

**F.3.1.2.2.3.2 通过要求**

试验后，读取组合驾驶辅助数据记录系统记录的事件数据，组合驾驶辅助数据记录系统对于事件的触发应符合F.1.2.2.3的要求。

**F.3.1.2.2.4 对于分布式数据记录系统**

**F.3.1.2.2.4.1 试验方法**

对于配备采用分布式模块实现的I型系统的试验车辆，按照GB 39732—2020中5.3.2的方法对其中需由加速度触发记录的模块进行试验，验证组合驾驶辅助数据记录系统中与该模块有关部分数据，之后在已激活组合驾驶辅助系统的整车上注入台架试验模拟信号，待组合驾驶辅助数据记录系统完成本次记录后，试验终止。

**F.3.1.2.2.4.2 通过要求**

试验后，读取组合驾驶辅助数据记录系统各分布式模块记录的事件数据，组合驾驶辅助数据记录系统对于事件的触发应符合F.1.2.2.3的要求。

##### F.3.1.3 有碰撞风险事件触发试验

###### F.3.1.3.1 试验场景

测试道路为至少包含两条车道的长直道，中间车道线为白色虚线。试验车辆和车辆目标在各自车道内行驶，在试验车辆接近车辆目标过程中，车辆目标切入试验车辆所在车道，如图F.1所示。

###### F.3.1.3.2 试验方法

对于配备I型系统的试验车辆，激活组合驾驶辅助系统后，试验车辆在车道内稳定运行一段时间，并在距离相邻车道目标物200 m处开始试验，在试验车辆最前端与车辆目标最后端碰撞时间（TTC）为1.5 s到3 s时，车辆目标快速切入试验车辆所在车道，并沿车道中间行驶。

> **注：** 若该场景不能触发有碰撞风险事件，需由车辆制造商提供触发有碰撞风险事件的试验场景及试验参数。

###### F.3.1.3.3 通过要求

试验后，读取组合驾驶辅助数据记录系统记录的数据，组合驾驶辅助数据记录系统对于事件的触发应符合F.1.2.3.1和F.1.2.3.3的要求。

<div align="center">
  <img src="../images/figures/figure-f1.png" alt="图f1" style="width: 14cm">
  <br>
  <strong>图F.1 有碰撞风险事件试验场景示意图</strong>
</div>

#### F.3.2 连续记录触发试验

##### F.3.2.1 试验方法

对于配备II型系统的试验车辆按照F.3.1.1.1进行试验。

##### F.3.2.2 通过要求

试验后，读取组合驾驶辅助数据记录系统记录的数据，应符合F.1.3 a)和b）的要求。

#### F.3.3 碰撞试验

##### F.3.3.1 试验条件

试验前，读取试验车辆的组合驾驶辅助数据记录系统已存储的数据。

##### F.3.3.2 试验方法

对于M₁类和N₁类车辆，应按照如下要求进行试验：

> —— 如适用GB 11551或GB/T 20913，按照GB 11551或GB/T 20913进行正面或正面偏置碰撞试验；

> —— 如适用GB 20071，按照GB 20071进行侧面碰撞试验。

##### F.3.3.3 通过要求

试验后，读取组合驾驶辅助数据记录系统存储的数据，与试验前读取的数据进行比对，符合F.1.8的要求。

#### F.3.4 数据准确性验证试验

##### F.3.4.1 试验方法

对于配备I型系统的试验车辆，按照F.3.1.3.2进行试验；对于配备II型系统的试验车辆，按照F.3.2.1进行试验。

##### F.3.4.2 通过要求

试验后，读取组合驾驶辅助数据记录系统中记录的数据，并与相应的测量值进行比对，应符合F.1.4.2中除表F.3和表F.4以外的其他要求。

#### F.3.5 数据存储机制试验

##### F.3.5.1 连续存储能力试验

###### F.3.5.1.1 试验方法

对于配备II型系统的试验车辆，激活试验车辆组合驾驶辅助系统并完成累计不少于8 h的运行。

###### F.3.5.1.2 通过要求

试验后，读取组合驾驶辅助数据记录系统记录的数据，应符合F.1.5.2中b）的要求。

##### F.3.5.2 存储能力及覆盖机制试验

###### F.3.5.2.1 时间戳事件存储覆盖试验

**F.3.5.2.1.1 试验方法**

按照F.3.1.1.1进行1次试验。

**F.3.5.2.1.2 通过要求**

试验后，读取组合驾驶辅助数据记录系统存储的数据，应符合F.1.5.3的要求。

###### F.3.5.2.2 时间段事件存储能力及覆盖试验

**F.3.5.2.2.1 试验方法**

按照F.3.1.2或F.3.1.3进行试验。

**F.3.5.2.2.2 通过要求**

试验后，读取组合驾驶辅助数据记录系统记录的数据，应满足F.1.5.2a）和F.1.5.3.1中除e）以外的要求。

#### F.3.5.3 断电存储试验

##### F.3.5.3.1 试验方法

组合驾驶辅助数据记录系统稳定运行不少于15 s，按照F.3.1.2或F.3.1.3进行试验，5 s后切断一条组合驾驶辅助数据记录系统的供电线路、记录切断电路的时刻点并重新上电。

##### F.3.5.3.2 通过要求

试验后，读取组合驾驶辅助数据记录系统记录的数据，应满足F.1.5.4的要求。

#### F.3.6 环境评价性试验

##### F.3.6.1 电气性能

###### F.3.6.1.1 直流供电电压

以GB/T 28046.1—2011定义的工作模式3.1，先将直流稳压电源电压调至 *U<sub>N</sub>*，然后逐渐将电压调至 *U<sub>Smin</sub>* 稳定10 min，再逐渐将电压调至 *U<sub>Smax</sub>* 稳定10 min，试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.1.2 过电压

**F.3.6.1.2.1（*T<sub>max</sub>*-20℃）条件**

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.2—2019中4.3.1.1.2或4.3.2.2的方法进行试验。

*U<sub>N</sub>* 为12 V时，在温度试验箱中将实现组合驾驶辅助数据记录系统功能的ECU加热到 *T*=（*T<sub>max</sub>*-20℃），向电源输入端施加18 V±0.2 V的电压持续（60 ±1）min。*U<sub>N</sub>* 为24 V时，在温度试验箱中将实现组合驾驶辅助数据记录系统功能的ECU加热到 *T*=（*T<sub>max</sub>*-20℃），向电源输入端施加（36±0.2）V的电压持续（60±1）min。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

**F.3.6.1.2.2 室温条件下**

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.2—2019中4.3.1.2.2的方法进行试验。

*U<sub>N</sub>* 为12 V时，将直流稳压电源调至（24±0.25）V，保持（60±6）s。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.1.3 叠加交流电压

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.2—2019中4.4.2严酷度1的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.1.4 供电电压缓降和缓升

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.2—2019中4.5.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.1.5 供电电压瞬态变化

**F.3.6.1.5.1 电压瞬时下降**

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.2—2019中4.6.1.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

**F.3.6.1.5.2 对电压骤降的复位性能**

以GB/T 28046.1—2011定义的工作模式3.1,按照GB/T 28046.2—2019中4.6.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

**F.3.6.1.5.3 启动特性**

以GB/T 28046.1—2011定义的工作模式3.1,按照GB/T 28046.2—2019中4.6.3.2等级Ⅱ的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

**F.3.6.1.5.4 抛负载**

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.2—2019中4.6.4.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.1.6 反向电压

以GB/T 28046.1—2011定义的工作模式3.1,按表F.9的方法进行试验。其他电压规格系统的试验条件可协商确定。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

<div align="center">
  <strong>表F.9 反向电压试验</strong>

<table>
<thead>
  <tr>
    <th align="center">序号</th>
    <th align="center">名称</th>
    <th align="center" colspan="2">试验参数</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">1</td>
    <td align="center">U<sub>N</sub></td>
    <td align="center">12 V</td>
    <td align="center">24 V</td>
  </tr>
  <tr>
    <td align="center">2</td>
    <td align="center">试验电压（电源输入接口正负极反接）</td>
    <td align="center">-14 V</td>
    <td align="center">-28 V</td>
  </tr>
  <tr>
    <td align="center">3</td>
    <td align="center">试验时间</td>
    <td align="center" colspan="2">(60±6) s</td>
  </tr>
  <tr>
    <td align="center">4</td>
    <td align="center">试验循环次数</td>
    <td align="center" colspan="2">1次</td>
  </tr>
</tbody>
</table>

</div>

###### F.3.6.1.7 参考接地和供电偏移

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.2—2019中4.8.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.1.8 开路

**F.3.6.1.8.1 单线开路**

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.2—2019中4.9.1.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

**F.3.6.1.8.2 多线开路**

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.2—2019中4.9.2.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.1.9 短路保护

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.2—2019中4.10.2.1的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.1.10 绝缘电阻

以GB/T 28046.1—2011定义的工作模式1.1，按照GB/T 28046.2—2019中4.12.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

##### F.3.6.2 防尘防水性能

以GB/T 28046.1—2011定义的工作模式1.1，按照GB/T 30038—2013中8.3.3.2和8.4.3的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

##### F.3.6.3 环境耐候性

###### F.3.6.3.1 低温贮存

在低温-40 ℃贮存并以GB/T 28046.1—2011定义的工作模式1.1，按照GB/T 28046.4—2011中5.1.1.1.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.3.2 低温工作

以最低工作温度（*T<sub>min</sub>*）和GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.4—2011中5.1.1.2.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.3.3 高温贮存

在高温85 ℃贮存并以GB/T 28046.1—2011定义的工作模式1.1，按照GB/T 28046.4—2011中5.1.2.1.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.3.4 高温工作

以最高工作温度（*T<sub>max</sub>*）和GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.4—2011中5.1.2.2.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.3.5 温度梯度

在 *T<sub>min</sub>* ～ *T<sub>max</sub>* 范围内和GB/T 28046.1-2011定义的工作模式3.1，按照GB/T 28046.4—2011中5.2.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.3.6 规定转换时间的温度快速变化

在 *T<sub>min</sub>* ～ *T<sub>max</sub>* 范围内和GB/T 28046.1-2011定义的工作模式1.1，按照GB/T 28046.4—2011中5.3.2.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.3.7 规定变化率的温度循环

在 *T<sub>min</sub>* ～ *T<sub>max</sub>* 范围内和GB/T 28046.1-2011定义的工作模式3.1，按照GB/T 28046.4—2011中的5.3.1.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.3.8 湿热循环

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.4—2011中5.6.2.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.3.9 稳态湿热

以GB/T 28046.1—2011定义的工作模式2.1（试验最后1 h采用GB/T 28046.1—2011定义的工作模式3.1），按照GB/T 28046.4—2011中5.7.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.3.10 太阳光辐射

安装在乘客舱内太阳直射处的组合驾驶辅助数据记录系统，以GB/T 28046.1—2011定义的工作模式1.1，按照GB/T 1865—2009中方法2和表3循环C进行600 h试验。

试验后，检查实现组合驾驶辅助数据记录系统功能的控制器表面。

##### F.3.6.4 机械性能

###### F.3.6.4.1 机械振动

模拟在车辆上的安装方式在振动台上安装固定，以GB/T 28046.1—2011定义的工作模式3.1，根据不同安装位置，按照GB/T 28046.3—2011中4.1.2.4.2、4.1.2.7.2或4.1.2.8.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.4.2 机械冲击

以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 28046.3—2011中4.2.2.2的方法进行试验。试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

##### F.3.6.5 化学负荷

组合驾驶辅助数据记录系统以GB/T 28046.1—2011定义的工作模式1.1，按照GB/T 28046.5—2013中表1安装位置代码[B]选择试剂和暴露条件以及表2的湿润方法和4.8的程序进行试验。

试验后，检查实现组合驾驶辅助数据记录系统功能的控制器表面，读取并检查组合驾驶辅助数据记录系统中存储的数据。

##### F.3.6.6 电磁兼容性能

###### F.3.6.6.1 对静电放电产生的电骚扰抗扰

**F.3.6.6.1.1 电子模块不通电**

组合驾驶辅助数据记录系统以GB/T 28046.1—2011定义的工作模式1.1，按照GB/T 19951-2019附录C中表C.1、表C.2 的类别1试验严酷等级不低于L3的测试电压要求和第9章规定的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

**F.3.6.6.1.2 电子模块通电**

组合驾驶辅助数据记录系统以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 19951—2019附录C中表C.1、表C.2、表C.3的类别1试验严酷等级不低于L3的测试电压要求和第8章规定的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.6.2 对由传导和耦合引起的电骚扰抗扰

**F.3.6.6.2.1 沿电源线的电瞬态传导抗扰**

组合驾驶辅助数据记录系统以GB/T 28046.1—2011定义的工作模式3.1，按照表F.8规定的抗扰试验等级和GB 34660-2017中5.8的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

**F.3.6.6.2.2 除电源线外的导线通过容性和感性耦合的电瞬态抗扰**

组合驾驶辅助数据记录系统以GB/T 28046.1—2011定义的工作模式3.1，按照GB/T 21437.3—2021中表B.1、表B.2中CCC和ICC模式以及等级Ⅲ的要求和3.4.2的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.6.3 对电磁辐射的抗扰

组合驾驶辅助数据记录系统以GB/T 28046.1—2011定义的工作模式3.1, 按照GB 34660—2017中4.7的电波暗室法、大电流注入法的抗扰试验强度和5.7的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

###### F.3.6.6.4 无线电骚扰特性

组合驾驶辅助数据记录系统以GB/T 28046.1—2011定义的工作模式3.1，按照GB 34660—2017中5.5和5.6的方法进行试验。

试验后，读取并检查组合驾驶辅助数据记录系统中存储的数据。

#### F.3.7 信息安全试验

对组合驾驶辅助数据记录系统的访问接口进行攻击操作，若无法实现篡改和非授权删除存储的数据，则试验通过，否则依次进行如下试验：对存储的数据进行篡改和非授权删除操作，并读取数据，若在读取时有篡改、非授权删除操作的记录，则试验通过，否则不通过。

### F.4 基于CAN线通信的数据元素排列要求

<div align="center">
  <strong>表F.10 基于CAN线通信的时间戳数据元素排列</strong>

<table>
<thead>
  <tr>
    <th align="center">ID</th>
    <th align="center">名称</th>
    <th align="center">单位</th>
    <th align="center">记录等级</th>
    <th align="center">单个信号长度 bit</th>
    <th align="center">单个信号长度 byte</th>
    <th align="center">单个事件信号数量</th>
    <th align="center">单个事件信号长度 byte</th>
    <th align="center">字节序列号</th>
    <th align="center">转化公式</th>
    <th align="center">无法获取值</th>
    <th align="center">无效值</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center" rowspan="13">0xFA51</td>
    <td align="center">车辆识别代号（VIN）</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">136</td>
    <td align="center">17</td>
    <td align="center">1</td>
    <td align="center">17</td>
    <td align="center">0~16</td>
    <td align="center">ASCII</td>
    <td align="center">17个字节均填充 FF<sub>16</sub></td>
    <td align="center">前16个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">实现组合驾驶辅助数据记录系统功能的硬件型号</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">160</td>
    <td align="center">20</td>
    <td align="center">1</td>
    <td align="center">20</td>
    <td align="center">17~36</td>
    <td align="center">ASCII，字节数小于20时，应用0x20填充，填充位在左边</td>
    <td align="center">20个字节均填充 FF<sub>16</sub></td>
    <td align="center">前19个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">实现组合驾驶辅助数据记录系统功能的硬件序列号</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">160</td>
    <td align="center">20</td>
    <td align="center">1</td>
    <td align="center">20</td>
    <td align="center">37~56</td>
    <td align="center">ASCII，字节数小于20时，应用0x20填充，填充位在左边</td>
    <td align="center">20个字节均填充 FF<sub>16</sub></td>
    <td align="center">前19个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统软件版本号</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">160</td>
    <td align="center">20</td>
    <td align="center">1</td>
    <td align="center">20</td>
    <td align="center">57~76</td>
    <td align="center">ASCII，字节数小于20 时, 应用0x20填充, 填充位在左边</td>
    <td align="center">20个字节均填充 FF<sub>16</sub></td>
    <td align="center">前19个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助数据记录系统软件版本号</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">160</td>
    <td align="center">20</td>
    <td align="center">1</td>
    <td align="center">20</td>
    <td align="center">77~96</td>
    <td align="center">ASCII，字节数小于20 时, 应用0x20填充, 填充位在左边</td>
    <td align="center">20个字节均填充 FF<sub>16</sub></td>
    <td align="center">前19个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
    <tr>
    <td align="center">事件类型编码</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">97</td>
    <td align="left">0x07：锁定碰撞<br/>0x10：非锁定碰撞<br/>0x14：有碰撞风险<br/>0x15：组合驾驶辅助系统部分激活<br/>0x16：组合驾驶辅助系统激活<br/>0x17：组合驾驶辅助系统主动退出<br/>0x18：用户操纵组合驾驶辅助系统退出<br/>0x19：组合驾驶辅助系统发出HOR提示信号<br/>0x1a：组合驾驶辅助系统消除HOR提示或警告信号<br/>0x1b：组合驾驶辅助系统发出EOR提示信号<br/>0x1c：组合驾驶辅助系统消除EOR提示或警告信号<br/>0x1d：发出DCA<br/>0x1e：开始执行RMF<br/>0x1f：组合驾驶辅助系统严重失效<br/>0x20：车辆严重失效</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">累计行驶里程</td>
    <td align="center">km</td>
    <td align="center">A</td>
    <td align="center">32</td>
    <td align="center">4</td>
    <td align="center">1</td>
    <td align="center">4</td>
    <td align="center">98~101</td>
    <td align="center">E = N<br/>有效值范围：0-2000000</td>
    <td align="center">4个字节均填充 FF<sub>16</sub></td>
    <td align="center">前3个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">年</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">102</td>
    <td align="center">E=N+2000</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">月</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">103</td>
    <td align="center">E=N</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">日</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">104</td>
    <td align="center">E=N</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">时</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">105</td>
    <td align="center">E=N</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">分</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">106</td>
    <td align="center">E=N</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">秒</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">107</td>
    <td align="center">E=N</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center" rowspan="57">0xFA61<br/>0xFA62<br/>0xFA63<br/>0xFA64<br/>0xFA65</td>
    <td align="center">车辆识别代号（VIN）</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">136</td>
    <td align="center">17</td>
    <td align="center">1</td>
    <td align="center">17</td>
    <td align="center">0~16</td>
    <td align="center">ASCII</td>
    <td align="center">17个字节均填充 FF<sub>16</sub></td>
    <td align="center">前16个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">实现组合驾驶辅助数据记录系统功能的硬件型号</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">160</td>
    <td align="center">20</td>
    <td align="center">1</td>
    <td align="center">20</td>
    <td align="center">17~36</td>
    <td align="center">ASCII，字节数小于20时，应用0x20填充，填充位在左边</td>
    <td align="center">20个字节均填充 FF<sub>16</sub></td>
    <td align="center">前19个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">实现组合驾驶辅助数据记录系统功能的硬件序列号</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">160</td>
    <td align="center">20</td>
    <td align="center">1</td>
    <td align="center">20</td>
    <td align="center">37~56</td>
    <td align="center">ASCII，字节数小于20时，应用0x20填充，填充位在左边</td>
    <td align="center">20个字节均填充 FF<sub>16</sub></td>
    <td align="center">前19个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统软件版本号</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">160</td>
    <td align="center">20</td>
    <td align="center">1</td>
    <td align="center">20</td>
    <td align="center">57~76</td>
    <td align="center">ASCII，字节数小于20时，应用0x20填充，填充位在左边</td>
    <td align="center">20个字节均填充 FF<sub>16</sub></td>
    <td align="center">前19个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助数据记录系统软件版本号</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">160</td>
    <td align="center">20</td>
    <td align="center">1</td>
    <td align="center">20</td>
    <td align="center">77~96</td>
    <td align="center">ASCII，字节数小于20时，应用0x20填充，填充位在左边</td>
    <td align="center">20个字节均填充 FF<sub>16</sub></td>
    <td align="center">前19个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">事件类型编码</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">97</td>
    <td align="left">0x07：锁定碰撞<br/>0x10：非锁定碰撞<br/>0x14：有碰撞风险<br/>0x15：组合驾驶辅助系统部分激活<br/>0x16：组合驾驶辅助系统激活<br/>0x17：组合驾驶辅助系统主动退出<br/>0x18：用户操纵组合驾驶辅助系统退出<br/>0x19：组合驾驶辅助系统发出HOR提示信号<br/>0x1a：组合驾驶辅助系统消除HOR提示或警告信号<br/>0x1b：组合驾驶辅助系统发出EOR提示信号<br/>0x1c：组合驾驶辅助系统消除EOR提示或警告信号<br/>0x1d：发出DCA<br/>0x1e：开始执行RMF<br/>0x1f：组合驾驶辅助系统严重失效<br/>0x20：车辆严重失效</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">累计行驶里程</td>
    <td align="center">km</td>
    <td align="center">A</td>
    <td align="center">32</td>
    <td align="center">4</td>
    <td align="center">1</td>
    <td align="center">4</td>
    <td align="center">98~101</td>
    <td align="center">E = N<br/>有效值范围：0~2000000</td>
    <td align="center">4个字节均填充 FF<sub>16</sub></td>
    <td align="center">前3个字节填充 FF<sub>16</sub>，最后一个字节填充 FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">连续多次时间段事件的事件类型</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">102</td>
    <td align="center">00x07：锁定碰撞<br/>0x10：非锁定碰撞<br/>0x14：有碰撞风险</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">连续多次时间段事件的事件起点时刻</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">1</td>
    <td align="center">2</td>
    <td align="center">103~104</td>
    <td align="center">E = N<br/>时间应采用UTC时间，格式为自"1970-01-01 00:00:00"起经过的毫秒数</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">事件记录完整标志</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">105</td>
    <td align="center">1：完整<br/>0：不完整</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">车辆速度</td>
    <td align="center">km/h</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">200</td>
    <td align="center">400</td>
    <td align="center">106~505</td>
    <td align="center">E = N<br/>范围：[0, 300 km/h]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">车辆横向加速度</td>
    <td align="center">m/s²</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">200</td>
    <td align="center">400</td>
    <td align="center">506~905</td>
    <td align="center">E = N - 3000<br/>范围：[-3000 m/s², 3000 m/s²]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">车辆纵向加速度</td>
    <td align="center">m/s²</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">200</td>
    <td align="center">400</td>
    <td align="center">906~1305</td>
    <td align="center">E = N - 3000<br/>范围：[-3000 m/s², 3000 m/s²]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">车辆横摆角速度</td>
    <td align="center">°/s</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">40</td>
    <td align="center">80</td>
    <td align="center">1306~1385</td>
    <td align="center">E = N×0.1 - 3000<br/>范围：[-3000 °/s, 3000 °/s²]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">车辆侧倾角速度</td>
    <td align="center">°/s</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">40</td>
    <td align="center">80</td>
    <td align="center">1336~1465</td>
    <td align="center">E = N×0.1 - 3000<br/>范围：[-3000°/s, 3000°/s]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">航向角</td>
    <td align="center">°</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">40</td>
    <td align="center">80</td>
    <td align="center">1466~1545</td>
    <td align="center">E = N - 180<br/>范围：[-180°, 180°]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">转向盘角度</td>
    <td align="center">°</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">40</td>
    <td align="center">80</td>
    <td align="center">1546~1625</td>
    <td align="center">E = N×5 - 250<br/>范围：[-250°, 250°]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的横向加速度</td>
    <td align="center">m/s²</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">1626~1785</td>
    <td align="center">E = N×0.5 - 20<br/>范围：[-20 m/s², 20 m/s²]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的转向盘转向角</td>
    <td align="center">°</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">1786~1845</td>
    <td align="center">E = N-780<br/>范围：[-780°, 780°]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的转向曲率</td>
    <td align="center">1/m</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">1846~2005</td>
    <td align="center">E = N×0.001 - 0.2<br/>范围：[-780°, 780°]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的前轮转角</td>
    <td align="center">°</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">2006~2165</td>
    <td align="center">E = N×0.1-80<br/>范围：[-80°, 80°]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的转向小齿轮转向角</td>
    <td align="center">°</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">2166~2325</td>
    <td align="center">E = N×0.005-163<br/>范围：[-163°, 164°]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的转向盘转向力矩</td>
    <td align="center">Nm</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">2326~2485</td>
    <td align="center">E = N×0.1-11<br/>范围：[-11Nm, 11Nm]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的转向盘转向角速率</td>
    <td align="center">°/s</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">2486~2545</td>
    <td align="center">E = N×10<br/>范围：[0°/s, 200°/s]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的车速</td>
    <td align="center">km/h</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">2546~2705</td>
    <td align="center">E= N<br/>范围：[0,300 km/h]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的纵向加速度</td>
    <td align="center">m/s²</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">2706~2865</td>
    <td align="center">E = N×0.5 - 20<br/>范围：[-20 m/s², 20 m/s²]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的加速踏板开度比例</td>
    <td align="center">%</td>
    <td align="center">B</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">80</td>
    <td align="center">80</td>
    <td align="center">2866~2945</td>
    <td align="center">E = N<br/>范围：[0%, 100%]</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的刹车踏板开度比例</td>
    <td align="center">%</td>
    <td align="center">B</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">80</td>
    <td align="center">80</td>
    <td align="center">2946~3025</td>
    <td align="center">E = N<br/>范围：[0%~100%]</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的驱动转矩</td>
    <td align="center">Nm</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">3026~3185</td>
    <td align="center">E = N-1000<br/>范围：[-1000Nm, 1000Nm]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的驱动转速</td>
    <td align="center">rpm</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">3186~3345</td>
    <td align="center">E = N×100-50000<br/>范围：[-50000rpm, 200000rpm]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的轮端扭矩</td>
    <td align="center">Nm</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">3346~3505</td>
    <td align="center">E = N-32767<br/>范围：[-32767Nm, 32768 Nm]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的制动主缸压力</td>
    <td align="center">MPa</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">3506~3665</td>
    <td align="center">E=N<br/>范围：[0, 12MPa]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的挡位</td>
    <td align="center">不适用</td>
    <td align="center">B</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">80</td>
    <td align="center">80</td>
    <td align="center">3666~3745</td>
    <td align="center">1：P 挡<br/>2：R 挡<br/>3：N 挡<br/>4：D挡</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的车辆灯光状态</td>
    <td align="center">不适用</td>
    <td align="center">B</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">80</td>
    <td align="center">160</td>
    <td align="center">3746~3905</td>
    <td align="left">自左向右每位表示灯光的开关状态，00表示关闭，01表示打开，10表示告警，11表示无效：<br/>bit 0-1：自适应照明系统<br/>bit 2-3：近光灯<br/>bit 4-5：远光灯<br/>bit 6-7：危险警示灯<br/>bit 8-9：左转向灯<br/>bit 10-11：右转向灯</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">组合驾驶辅助系统请求的车辆雨刮状态</td>
    <td align="center">不适用</td>
    <td align="center">B</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">80</td>
    <td align="center">80</td>
    <td align="center">3906~3985</td>
    <td align="center">1：开启<br/>0：关闭</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">感知目标物ID</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">200</td>
    <td align="center">400</td>
    <td align="center">3986~4385</td>
    <td align="center">E = N</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">感知目标物类型</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">200</td>
    <td align="center">400</td>
    <td align="center">4386~4785</td>
    <td align="left">0x01：弱势道路参与者<br/>0x02：小型车<br/>0x03：大型车<br/>0x04：其他</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">感知目标物相对位置（X向）</td>
    <td align="center">m</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">200</td>
    <td align="center">400</td>
    <td align="center">4786~5185</td>
    <td align="center">E = N×0.5-1500；<br/>范围：[-1500m, 1500m]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">感知目标物相对位置（Y向）</td>
    <td align="center">m</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">200</td>
    <td align="center">400</td>
    <td align="center">5186~5585</td>
    <td align="center">E = N×0.5-1000；<br/>范围：[-1000m, 1000m]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">感知目标物相对速度（X向）</td>
    <td align="center">km/h</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">200</td>
    <td align="center">400</td>
    <td align="center">5586~5985</td>
    <td align="center">E = N×0.1-300；<br/>范围：[-300km/h, 300km/h]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">感知目标物相对速度（Y向）</td>
    <td align="center">km/h</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">200</td>
    <td align="center">400</td>
    <td align="center">5986~6385</td>
    <td align="center">E = N×0.1-300；<br/>范围：[-300km/h, 300km/h]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">驾驶员是否系安全带</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">40</td>
    <td align="center">40</td>
    <td align="center">6386~6425</td>
    <td align="left">0：未系安全带<br/>1：系安全带</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">驾驶员是否在驾驶位置</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">40</td>
    <td align="center">40</td>
    <td align="center">6426~6465</td>
    <td align="center">0：否<br/>1：是</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">驾驶员是否脱手</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">40</td>
    <td align="center">40</td>
    <td align="center">6466~6505</td>
    <td align="center">0：否<br/>1：是</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">驾驶员是否视线脱离</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">40</td>
    <td align="center">40</td>
    <td align="center">6506~6545</td>
    <td align="center">0：否<br/>1：是</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">加速踏板开度</td>
    <td align="center">%</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">40</td>
    <td align="center">40</td>
    <td align="center">6546~6585</td>
    <td align="center">E = N<br/>范围：[0%, 100%]</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">制动踏板开度<sup>a, b</sup></td>
    <td align="center">%</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">40</td>
    <td align="center">40</td>
    <td align="center">6586~6625</td>
    <td align="center">E = N<br/>范围：[0%, 100%]</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">输入转向扭矩<sup>d</sup></td>
    <td align="center">Nm</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">40</td>
    <td align="center">80</td>
    <td align="center">6626~6705</td>
    <td align="center">E = N×0.1<br/>范围：[-10, 10Nm]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">系统激活后用户设置巡航车速</td>
    <td align="center">km/h</td>
    <td align="center">A</td>
    <td align="center">16</td>
    <td align="center">2</td>
    <td align="center">40</td>
    <td align="center">80</td>
    <td align="center">6706~6785</td>
    <td align="center">E = N<br/>范围：[0, 240km/h]</td>
    <td align="center">FFFF<sub>16</sub></td>
    <td align="center">FFFE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">年</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">6786</td>
    <td align="center">E=N+2000</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">月</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">6787</td>
    <td align="center">E=N</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">日</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">6788</td>
    <td align="center">E=N</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">时</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">6789</td>
    <td align="center">E=N</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">分</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">6790</td>
    <td align="center">E=N</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">秒</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center">8</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">1</td>
    <td align="center">6791</td>
    <td align="center">E=N</td>
    <td align="center">FF<sub>16</sub></td>
    <td align="center">FE<sub>16</sub></td>
  </tr>
  <tr>
    <td align="center">外部图像</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center">80</td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
  </tr>
  <tr>
    <td align="center">外部视频</td>
    <td align="center">不适用</td>
    <td align="center">A</td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center">80</td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
  </tr>
</tbody>
</table>

</div>