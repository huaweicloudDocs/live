# API概览<a name="topic_live_04_overview_100015"></a>

视频直播服务对应的接口列表如下所示，在调用视频直播API前，您需要先获取用户Token，Token可以用于调用其他API时鉴权，具体如何调用直播API请参考[快速入门](创建转码模板.md)。

## 转码模板管理接口<a name="zh-cn_topic_0140252983_section1490691275720"></a>

**表 1**  转码模板管理接口

<a name="zh-cn_topic_0140252983_table182059123588"></a>
<table><thead align="left"><tr id="zh-cn_topic_0140252983_row1520651265819"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0140252983_p120881213585"><a name="zh-cn_topic_0140252983_p120881213585"></a><a name="zh-cn_topic_0140252983_p120881213585"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0140252983_p520851285811"><a name="zh-cn_topic_0140252983_p520851285811"></a><a name="zh-cn_topic_0140252983_p520851285811"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0140252983_row162091912185820"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p621119122585"><a name="zh-cn_topic_0140252983_p621119122585"></a><a name="zh-cn_topic_0140252983_p621119122585"></a>POST /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p32120125581"><a name="zh-cn_topic_0140252983_p32120125581"></a><a name="zh-cn_topic_0140252983_p32120125581"></a><a href="创建直播转码模板.md">创建直播转码模板</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row10212111285820"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p521341265816"><a name="zh-cn_topic_0140252983_p521341265816"></a><a name="zh-cn_topic_0140252983_p521341265816"></a>DELETE /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p9215201235816"><a name="zh-cn_topic_0140252983_p9215201235816"></a><a name="zh-cn_topic_0140252983_p9215201235816"></a><a href="删除直播转码模板.md">删除直播转码模板</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row3216181215580"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p18217171217581"><a name="zh-cn_topic_0140252983_p18217171217581"></a><a name="zh-cn_topic_0140252983_p18217171217581"></a>PUT /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p1721961215816"><a name="zh-cn_topic_0140252983_p1721961215816"></a><a name="zh-cn_topic_0140252983_p1721961215816"></a><a href="配置直播转码模板.md">配置直播转码模板</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row11219121217581"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p9220141220583"><a name="zh-cn_topic_0140252983_p9220141220583"></a><a name="zh-cn_topic_0140252983_p9220141220583"></a>GET /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p522101215584"><a name="zh-cn_topic_0140252983_p522101215584"></a><a name="zh-cn_topic_0140252983_p522101215584"></a><a href="查询直播转码模板.md">查询直播转码模板</a></p>
</td>
</tr>
</tbody>
</table>

## 流管理接口<a name="zh-cn_topic_0140252983_section122718360575"></a>

**表 2**  流管理接口

<a name="zh-cn_topic_0140252983_table082712210581"></a>
<table><thead align="left"><tr id="zh-cn_topic_0140252983_row16829162285810"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0140252983_p1183072218581"><a name="zh-cn_topic_0140252983_p1183072218581"></a><a name="zh-cn_topic_0140252983_p1183072218581"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0140252983_p48311322205815"><a name="zh-cn_topic_0140252983_p48311322205815"></a><a name="zh-cn_topic_0140252983_p48311322205815"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0140252983_row1087624920495"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p98763498494"><a name="zh-cn_topic_0140252983_p98763498494"></a><a name="zh-cn_topic_0140252983_p98763498494"></a>GET /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p19876114904918"><a name="zh-cn_topic_0140252983_p19876114904918"></a><a name="zh-cn_topic_0140252983_p19876114904918"></a><a href="查询禁止直播推流列表.md">查询禁止直播推流列表</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row1536853762513"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p16369337182517"><a name="zh-cn_topic_0140252983_p16369337182517"></a><a name="zh-cn_topic_0140252983_p16369337182517"></a>PUT /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p83698370257"><a name="zh-cn_topic_0140252983_p83698370257"></a><a name="zh-cn_topic_0140252983_p83698370257"></a><a href="修改禁推属性.md">修改禁推属性</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row1784452213584"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p9845722125818"><a name="zh-cn_topic_0140252983_p9845722125818"></a><a name="zh-cn_topic_0140252983_p9845722125818"></a>POST /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p18462226585"><a name="zh-cn_topic_0140252983_p18462226585"></a><a name="zh-cn_topic_0140252983_p18462226585"></a><a href="禁止直播推流.md">禁止直播推流</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row130313472251"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p23041047172515"><a name="zh-cn_topic_0140252983_p23041047172515"></a><a name="zh-cn_topic_0140252983_p23041047172515"></a>DELETE /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p63041247182512"><a name="zh-cn_topic_0140252983_p63041247182512"></a><a name="zh-cn_topic_0140252983_p63041247182512"></a><a href="禁推恢复.md">禁推恢复</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row985342219586"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p1485452214582"><a name="zh-cn_topic_0140252983_p1485452214582"></a><a name="zh-cn_topic_0140252983_p1485452214582"></a>GET /v1/{project_id}/stream/bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p158553227588"><a name="zh-cn_topic_0140252983_p158553227588"></a><a name="zh-cn_topic_0140252983_p158553227588"></a><a href="查询直播加速的带宽数据.md">查询直播加速的带宽数据</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row2855322115811"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p8857132211584"><a name="zh-cn_topic_0140252983_p8857132211584"></a><a name="zh-cn_topic_0140252983_p8857132211584"></a>GET /v1/{project_id}/stream/traffic</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p138581422195812"><a name="zh-cn_topic_0140252983_p138581422195812"></a><a name="zh-cn_topic_0140252983_p138581422195812"></a><a href="查询直播加速的流量数据.md">查询直播加速的流量数据</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row3858422185816"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p38582022135817"><a name="zh-cn_topic_0140252983_p38582022135817"></a><a name="zh-cn_topic_0140252983_p38582022135817"></a>GET /v1/{project_id}/stream/users</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p1886019228586"><a name="zh-cn_topic_0140252983_p1886019228586"></a><a name="zh-cn_topic_0140252983_p1886019228586"></a><a href="查询直播播放在线人数.md">查询直播播放在线人数</a></p>
</td>
</tr>
</tbody>
</table>

## 录制管理接口<a name="zh-cn_topic_0140252983_section6534185517572"></a>

**表 3**  录制管理接口

<a name="zh-cn_topic_0140252983_table1991126205713"></a>
<table><thead align="left"><tr id="zh-cn_topic_0140252983_row16280735710"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0140252983_p112816711577"><a name="zh-cn_topic_0140252983_p112816711577"></a><a name="zh-cn_topic_0140252983_p112816711577"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0140252983_p18280785716"><a name="zh-cn_topic_0140252983_p18280785716"></a><a name="zh-cn_topic_0140252983_p18280785716"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0140252983_row20314717576"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p1631177165712"><a name="zh-cn_topic_0140252983_p1631177165712"></a><a name="zh-cn_topic_0140252983_p1631177165712"></a>POST /v1/{project_id}/record/config</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p173111785710"><a name="zh-cn_topic_0140252983_p173111785710"></a><a name="zh-cn_topic_0140252983_p173111785710"></a><a href="创建录制配置.md">创建录制配置</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row1331775573"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p1933197115719"><a name="zh-cn_topic_0140252983_p1933197115719"></a><a name="zh-cn_topic_0140252983_p1933197115719"></a>GET /v1/{project_id}/record/config</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p1133873574"><a name="zh-cn_topic_0140252983_p1133873574"></a><a name="zh-cn_topic_0140252983_p1133873574"></a><a href="查询录制配置.md">查询录制配置</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row1633071574"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p53317710573"><a name="zh-cn_topic_0140252983_p53317710573"></a><a name="zh-cn_topic_0140252983_p53317710573"></a>DELETE /v1/{project_id}/record/config</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p13316716571"><a name="zh-cn_topic_0140252983_p13316716571"></a><a name="zh-cn_topic_0140252983_p13316716571"></a><a href="删除录制配置.md">删除录制配置</a></p>
</td>
</tr>
</tbody>
</table>

