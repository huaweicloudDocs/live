# API概览<a name="topic_live_04_overview_100015"></a>

视频直播服务对应的接口列表如下所示，在调用视频直播API前，您需要先获取用户Token，Token可以用于调用其他API时鉴权，具体如何调用直播API请参考[快速入门](创建转码模板.md)。

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
<tr id="row1536853762513"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p16369337182517"><a name="p16369337182517"></a><a name="p16369337182517"></a>PUT /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p83698370257"><a name="p83698370257"></a><a name="p83698370257"></a><a href="修改禁推属性.md">修改禁推属性</a></p>
</td>
</tr>
<tr id="row1784452213584"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p9845722125818"><a name="p9845722125818"></a><a name="p9845722125818"></a>POST /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p18462226585"><a name="p18462226585"></a><a name="p18462226585"></a><a href="禁止直播推流.md">禁止直播推流</a></p>
</td>
</tr>
<tr id="row130313472251"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p23041047172515"><a name="p23041047172515"></a><a name="p23041047172515"></a>DELETE /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p63041247182512"><a name="p63041247182512"></a><a name="p63041247182512"></a><a href="恢复直播推流.md">恢复直播推流</a></p>
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

## 域名维度数据查询接口<a name="section136171539103810"></a>

**表 4**  域名维度数据查询接口

<a name="table1610917377392"></a>
<table><thead align="left"><tr id="row3109103783916"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p12109537183916"><a name="p12109537183916"></a><a name="p12109537183916"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p18109183711391"><a name="p18109183711391"></a><a name="p18109183711391"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17109153713395"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p12109193783916"><a name="p12109193783916"></a><a name="p12109193783916"></a>GET /v1/{project_id}/stats/domain/bandwidth/detail</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p610919372392"><a name="p610919372392"></a><a name="p610919372392"></a><a href="查询播放域名带宽趋势.md">查询播放域名带宽趋势</a></p>
</td>
</tr>
<tr id="row81091737163912"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p5109143753913"><a name="p5109143753913"></a><a name="p5109143753913"></a>GET /v1/{project_id}/stats/domain/traffic/detail</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p11109437153911"><a name="p11109437153911"></a><a name="p11109437153911"></a><a href="查询播放流量趋势.md">查询播放流量趋势</a></p>
</td>
</tr>
<tr id="row13109103773910"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p510983716395"><a name="p510983716395"></a><a name="p510983716395"></a>GET /v1/{project_id}/stats/domain/bandwidth/summary</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p710983713391"><a name="p710983713391"></a><a name="p710983713391"></a><a href="查询播放带宽峰值.md">查询播放带宽峰值</a></p>
</td>
</tr>
<tr id="row41092376395"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p310993718396"><a name="p310993718396"></a><a name="p310993718396"></a>GET /v1/{project_id}/stats/domain/traffic/summary</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1610963711399"><a name="p1610963711399"></a><a name="p1610963711399"></a><a href="查询播放流量汇总.md">查询播放流量汇总</a></p>
</td>
</tr>
</tbody>
</table>

## 流维度数据查询接口<a name="section10546145517389"></a>

**表 5**  流维度数据查询接口

<a name="table7139143874320"></a>
<table><thead align="left"><tr id="row121404387433"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p181401738204311"><a name="p181401738204311"></a><a name="p181401738204311"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p1914023884319"><a name="p1914023884319"></a><a name="p1914023884319"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row131406387435"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1614010389433"><a name="p1614010389433"></a><a name="p1614010389433"></a>GET /v1/{project_id}/monitor/streams</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p9140183816433"><a name="p9140183816433"></a><a name="p9140183816433"></a><a href="查询实时推流.md">查询实时推流</a></p>
</td>
</tr>
<tr id="row81401738204314"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p6140103894319"><a name="p6140103894319"></a><a name="p6140103894319"></a>GET /v1/{project_id}/stats/stream/user</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p21402386439"><a name="p21402386439"></a><a name="p21402386439"></a><a href="查询观众趋势.md">查询观众趋势</a></p>
</td>
</tr>
<tr id="row214043814430"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p17129629112112"><a name="p17129629112112"></a><a name="p17129629112112"></a>GET /v1/{project_id}/stats/stream/bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1214063874319"><a name="p1214063874319"></a><a name="p1214063874319"></a><a href="查询播放带宽趋势.md">查询播放带宽趋势</a></p>
</td>
</tr>
</tbody>
</table>

## 流监控接口<a name="section186134919393"></a>

**表 6**  流监控接口

<a name="table58515224617"></a>
<table><thead align="left"><tr id="row148782164610"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p2087182124620"><a name="p2087182124620"></a><a name="p2087182124620"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p087329465"><a name="p087329465"></a><a name="p087329465"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5877214464"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1351864182113"><a name="p1351864182113"></a><a name="p1351864182113"></a>GET /v1/{project_id}/stats/stream/framerate</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p208716294612"><a name="p208716294612"></a><a name="p208716294612"></a><a href="查询推流帧率数据.md">查询推流帧率数据</a></p>
</td>
</tr>
<tr id="row1087228461"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p108718216466"><a name="p108718216466"></a><a name="p108718216466"></a>GET /v1/{project_id}/stats/stream/bitrate</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p11871423460"><a name="p11871423460"></a><a name="p11871423460"></a><a href="查询推流码率数据.md">查询推流码率数据</a></p>
</td>
</tr>
<tr id="row48710210469"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1887821464"><a name="p1887821464"></a><a name="p1887821464"></a>GET /v1/{project_id}/stats/stream/timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p12879254612"><a name="p12879254612"></a><a name="p12879254612"></a><a href="查询拉流时间戳信息.md">查询拉流时间戳信息</a></p>
</td>
</tr>
</tbody>
</table>

