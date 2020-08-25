# API概览<a name="topic_live_04_overview_100015"></a>

视频直播服务对应的接口列表如下所示，在调用视频直播API前，您需要先获取用户Token，Token可以用于调用其他API时鉴权，具体如何调用直播API请参考[快速入门](示例1-创建转码模板.md)。

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
<tr id="row92461916298"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p18217171217581"><a name="zh-cn_topic_0140252983_p18217171217581"></a><a name="zh-cn_topic_0140252983_p18217171217581"></a>PUT /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p1721961215816"><a name="zh-cn_topic_0140252983_p1721961215816"></a><a name="zh-cn_topic_0140252983_p1721961215816"></a><a href="配置直播转码模板.md">配置直播转码模板</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row10212111285820"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p521341265816"><a name="zh-cn_topic_0140252983_p521341265816"></a><a name="zh-cn_topic_0140252983_p521341265816"></a>DELETE /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p9215201235816"><a name="zh-cn_topic_0140252983_p9215201235816"></a><a name="zh-cn_topic_0140252983_p9215201235816"></a><a href="删除直播转码模板.md">删除直播转码模板</a></p>
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
<tbody><tr id="row4182162262819"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p9845722125818"><a name="zh-cn_topic_0140252983_p9845722125818"></a><a name="zh-cn_topic_0140252983_p9845722125818"></a>POST /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p18462226585"><a name="zh-cn_topic_0140252983_p18462226585"></a><a name="zh-cn_topic_0140252983_p18462226585"></a><a href="禁止直播推流.md">禁止直播推流</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row1536853762513"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p16369337182517"><a name="zh-cn_topic_0140252983_p16369337182517"></a><a name="zh-cn_topic_0140252983_p16369337182517"></a>PUT /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p83698370257"><a name="zh-cn_topic_0140252983_p83698370257"></a><a name="zh-cn_topic_0140252983_p83698370257"></a><a href="修改禁推属性.md">修改禁推属性</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row130313472251"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p23041047172515"><a name="zh-cn_topic_0140252983_p23041047172515"></a><a name="zh-cn_topic_0140252983_p23041047172515"></a>DELETE /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p63041247182512"><a name="zh-cn_topic_0140252983_p63041247182512"></a><a name="zh-cn_topic_0140252983_p63041247182512"></a><a href="禁推恢复.md">禁推恢复</a></p>
</td>
</tr>
<tr id="row1657311423286"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0140252983_p98763498494"><a name="zh-cn_topic_0140252983_p98763498494"></a><a name="zh-cn_topic_0140252983_p98763498494"></a>GET /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p19876114904918"><a name="zh-cn_topic_0140252983_p19876114904918"></a><a name="zh-cn_topic_0140252983_p19876114904918"></a><a href="查询禁止直播推流列表.md">查询禁止直播推流列表</a></p>
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

## 数据统计分析接口<a name="zh-cn_topic_0140252983_section10546145517389"></a>

**表 4**  数据统计分析接口

<a name="zh-cn_topic_0140252983_table7139143874320"></a>
<table><thead align="left"><tr id="zh-cn_topic_0140252983_row121404387433"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0140252983_p181401738204311"><a name="zh-cn_topic_0140252983_p181401738204311"></a><a name="zh-cn_topic_0140252983_p181401738204311"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0140252983_p1914023884319"><a name="zh-cn_topic_0140252983_p1914023884319"></a><a name="zh-cn_topic_0140252983_p1914023884319"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0140252983_row131406387435"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p41901144195219"><a name="p41901144195219"></a><a name="p41901144195219"></a>GET /v2/{project_id}/stats/bandwidth/detail</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1718212495527"><a name="p1718212495527"></a><a name="p1718212495527"></a><a href="查询播放带宽趋势接口.md">查询播放带宽趋势</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row81401738204314"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p76968345533"><a name="p76968345533"></a><a name="p76968345533"></a>GET /v2/{project_id}/stats/traffic/detail</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0140252983_p21402386439"><a name="zh-cn_topic_0140252983_p21402386439"></a><a name="zh-cn_topic_0140252983_p21402386439"></a><a href="查询播放流量趋势接口.md">查询播放流量趋势</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row214043814430"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p12227328115315"><a name="p12227328115315"></a><a name="p12227328115315"></a>GET /v2/{project_id}/stats/bandwidth/peak</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p9981160175313"><a name="p9981160175313"></a><a name="p9981160175313"></a><a href="查询播放带宽峰值接口.md">查询播放带宽峰值</a></p>
</td>
</tr>
<tr id="row1425185175319"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p32516535311"><a name="p32516535311"></a><a name="p32516535311"></a>GET /v2/{project_id}/stats/traffic/summary</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p82617565316"><a name="p82617565316"></a><a name="p82617565316"></a><a href="查询播放流量汇总接口.md">查询播放流量汇总</a></p>
</td>
</tr>
<tr id="row119473105312"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p129493115316"><a name="p129493115316"></a><a name="p129493115316"></a>GET /v2/{project_id}/stats/user</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p094631537"><a name="p094631537"></a><a name="p094631537"></a><a href="查询观众趋势接口.md">查询观众趋势</a></p>
</td>
</tr>
<tr id="row598141117340"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p133858396226"><a name="p133858396226"></a><a name="p133858396226"></a>GET /v2/{project_id}/stats/httpcodes</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p58671473232"><a name="p58671473232"></a><a name="p58671473232"></a><a href="查询直播拉流HTTP状态码接口.md">查询直播拉流HTTP状态码接口</a></p>
</td>
</tr>
<tr id="row174991530436"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p139638597418"><a name="p139638597418"></a><a name="p139638597418"></a>GET /v2/{project_id}/stats/up-bandwidth/detail</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p2094953184410"><a name="p2094953184410"></a><a name="p2094953184410"></a><a href="查询上行带宽数据接口.md">查询上行带宽数据接口</a></p>
</td>
</tr>
<tr id="row8361135004316"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p8361750154319"><a name="p8361750154319"></a><a name="p8361750154319"></a>GET /v2/{project_id}/stats/stream-count</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1336114506438"><a name="p1336114506438"></a><a name="p1336114506438"></a><a href="查询域名维度推流路数接口.md">查询域名维度推流路数接口</a></p>
</td>
</tr>
<tr id="row79814964413"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p59864916446"><a name="p59864916446"></a><a name="p59864916446"></a>GET /v2/{project_id}/stats/history/streams</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p398149174419"><a name="p398149174419"></a><a name="p398149174419"></a><a href="查询历史推流列表接口.md">查询历史推流列表接口</a></p>
</td>
</tr>
</tbody>
</table>

## 流监控接口<a name="zh-cn_topic_0140252983_section186134919393"></a>

**表 5**  流监控接口

<a name="zh-cn_topic_0140252983_table58515224617"></a>
<table><thead align="left"><tr id="zh-cn_topic_0140252983_row148782164610"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0140252983_p2087182124620"><a name="zh-cn_topic_0140252983_p2087182124620"></a><a name="zh-cn_topic_0140252983_p2087182124620"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0140252983_p087329465"><a name="zh-cn_topic_0140252983_p087329465"></a><a name="zh-cn_topic_0140252983_p087329465"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0140252983_row5877214464"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p135861757195313"><a name="p135861757195313"></a><a name="p135861757195313"></a>GET /v2/{project_id}/stats/stream/framerate</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p528794365311"><a name="p528794365311"></a><a name="p528794365311"></a><a href="查询推流帧率数据接口.md">查询推流帧率数据</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0140252983_row1087228461"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p15600520545"><a name="p15600520545"></a><a name="p15600520545"></a>GET /v2/{project_id}/stats/stream/bitrate</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p10638165125319"><a name="p10638165125319"></a><a name="p10638165125319"></a><a href="查询推流码率数据接口.md">查询推流码率数据</a></p>
</td>
</tr>
</tbody>
</table>

