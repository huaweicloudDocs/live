# API概览<a name="ZH-CN_TOPIC_0140252983"></a>

视频直播服务对应的接口列表如下所示。

## 转码模板管理接口<a name="section1490691275720"></a>

**表 1**  转码模板管理接口

<a name="table182059123588"></a>
<table><thead align="left"><tr id="row1520651265819"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p120881213585"><a name="p120881213585"></a><a name="p120881213585"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p520851285811"><a name="p520851285811"></a><a name="p520851285811"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row162091912185820"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p621119122585"><a name="p621119122585"></a><a name="p621119122585"></a>POST /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p32120125581"><a name="p32120125581"></a><a name="p32120125581"></a><a href="创建直播转码模板.md">创建直播转码模板</a></p>
</td>
</tr>
<tr id="row10212111285820"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p521341265816"><a name="p521341265816"></a><a name="p521341265816"></a>DELETE /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p9215201235816"><a name="p9215201235816"></a><a name="p9215201235816"></a><a href="删除直播转码模板.md">删除直播转码模板</a></p>
</td>
</tr>
<tr id="row3216181215580"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p18217171217581"><a name="p18217171217581"></a><a name="p18217171217581"></a>PUT /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1721961215816"><a name="p1721961215816"></a><a name="p1721961215816"></a><a href="配置直播转码模板.md">配置直播转码模板</a></p>
</td>
</tr>
<tr id="row11219121217581"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p9220141220583"><a name="p9220141220583"></a><a name="p9220141220583"></a>GET /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p522101215584"><a name="p522101215584"></a><a name="p522101215584"></a><a href="查询直播转码模板.md">查询直播转码模板</a></p>
</td>
</tr>
</tbody>
</table>

## 流管理接口<a name="section122718360575"></a>

**表 2**  流管理接口

<a name="table082712210581"></a>
<table><thead align="left"><tr id="row16829162285810"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p1183072218581"><a name="p1183072218581"></a><a name="p1183072218581"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p48311322205815"><a name="p48311322205815"></a><a name="p48311322205815"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1087624920495"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p98763498494"><a name="p98763498494"></a><a name="p98763498494"></a>GET /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p19876114904918"><a name="p19876114904918"></a><a name="p19876114904918"></a><a href="查询禁推黑名单列表.md">查询禁推黑名单列表</a></p>
</td>
</tr>
<tr id="row1784452213584"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p9845722125818"><a name="p9845722125818"></a><a name="p9845722125818"></a>POST /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p18462226585"><a name="p18462226585"></a><a name="p18462226585"></a><a href="禁止直播推流.md">禁推（禁止直播推流）</a></p>
</td>
</tr>
<tr id="row0850202285812"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1485132235810"><a name="p1485132235810"></a><a name="p1485132235810"></a>GET /v1/{project_id}/stream/publish_list</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p26771514111917"><a name="p26771514111917"></a><a name="p26771514111917"></a><a href="查询直播推流列表（旧版）.md">查询直播推流列表（旧版）</a></p>
</td>
</tr>
<tr id="row54941555185111"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p16264526528"><a name="p16264526528"></a><a name="p16264526528"></a>GET /v1/{project_id}/origin/stream/statistic</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p249565511513"><a name="p249565511513"></a><a name="p249565511513"></a><a href="查询直播推流列表（新版）.md">查询直播推流列表（新版）</a></p>
</td>
</tr>
<tr id="row985342219586"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1485452214582"><a name="p1485452214582"></a><a name="p1485452214582"></a>GET /v1/{project_id}/stream/bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p158553227588"><a name="p158553227588"></a><a name="p158553227588"></a><a href="查询直播加速的带宽数据.md">查询直播加速的带宽数据</a></p>
</td>
</tr>
<tr id="row2855322115811"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p8857132211584"><a name="p8857132211584"></a><a name="p8857132211584"></a>GET /v1/{project_id}/stream/traffic</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p138581422195812"><a name="p138581422195812"></a><a name="p138581422195812"></a><a href="查询直播加速的流量数据.md">查询直播加速的流量数据</a></p>
</td>
</tr>
<tr id="row3858422185816"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p38582022135817"><a name="p38582022135817"></a><a name="p38582022135817"></a>GET /v1/{project_id}/stream/users</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1886019228586"><a name="p1886019228586"></a><a name="p1886019228586"></a><a href="查询直播播放在线人数.md">查询直播播放在线人数</a></p>
</td>
</tr>
</tbody>
</table>

## 录制管理接口<a name="section6534185517572"></a>

**表 3**  录制管理接口

<a name="table1991126205713"></a>
<table><thead align="left"><tr id="row16280735710"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p112816711577"><a name="p112816711577"></a><a name="p112816711577"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p18280785716"><a name="p18280785716"></a><a name="p18280785716"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row20314717576"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1631177165712"><a name="p1631177165712"></a><a name="p1631177165712"></a>POST /v1/{project_id}/record/config</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p173111785710"><a name="p173111785710"></a><a name="p173111785710"></a><a href="创建录制配置.md">创建录制配置</a></p>
</td>
</tr>
<tr id="row1331775573"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1933197115719"><a name="p1933197115719"></a><a name="p1933197115719"></a>GET /v1/{project_id}/record/config</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1133873574"><a name="p1133873574"></a><a name="p1133873574"></a><a href="查询录制配置.md">查询录制配置</a></p>
</td>
</tr>
<tr id="row1633071574"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p53317710573"><a name="p53317710573"></a><a name="p53317710573"></a>DELETE /v1/{project_id}/record/config</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p13316716571"><a name="p13316716571"></a><a name="p13316716571"></a><a href="删除录制配置.md">删除录制配置</a></p>
</td>
</tr>
</tbody>
</table>

