# API概览<a name="topic_live_04_overview_100015"></a>

视频直播服务对应的接口列表如下所示，在调用视频直播API前，您需要先获取用户Token，Token可以用于调用其他API时鉴权，具体如何调用直播API请参考[应用示例](示例1-创建转码模板.md)。

## 域名管理接口<a name="section221714381506"></a>

**表 1**  域名管理接口

<a name="table1790051419517"></a>
<table><thead align="left"><tr id="row1990041415516"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p129001914135110"><a name="p129001914135110"></a><a name="p129001914135110"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p59005144512"><a name="p59005144512"></a><a name="p59005144512"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1490013142511"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1790091417515"><a name="p1790091417515"></a><a name="p1790091417515"></a>POST /v1/{project_id}/domain</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p390041413517"><a name="p390041413517"></a><a name="p390041413517"></a><a href="创建直播域名.md">创建直播域名</a></p>
</td>
</tr>
<tr id="row790021416513"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p5900171413513"><a name="p5900171413513"></a><a name="p5900171413513"></a>DELETE /v1/{project_id}/domain</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p6901514135112"><a name="p6901514135112"></a><a name="p6901514135112"></a><a href="删除直播域名.md">删除直播域名</a></p>
</td>
</tr>
<tr id="row290171465117"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p15901314125112"><a name="p15901314125112"></a><a name="p15901314125112"></a>PUT /v1/{project_id}/domain</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p13901111410513"><a name="p13901111410513"></a><a name="p13901111410513"></a><a href="修改直播域名.md">修改直播域名</a></p>
</td>
</tr>
<tr id="row13901181410519"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1128412522223"><a name="p1128412522223"></a><a name="p1128412522223"></a>GET /v1/{project_id}/domain</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p69011614115118"><a name="p69011614115118"></a><a name="p69011614115118"></a><a href="查询直播域名.md">查询直播域名</a></p>
</td>
</tr>
<tr id="row1990151435112"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p990131410519"><a name="p990131410519"></a><a name="p990131410519"></a>PUT /v1/{project_id}/domains_mapping</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p0901121418512"><a name="p0901121418512"></a><a name="p0901121418512"></a><a href="域名映射.md">域名映射</a></p>
</td>
</tr>
<tr id="row13901111415110"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1890171417516"><a name="p1890171417516"></a><a name="p1890171417516"></a>DELETE /v1/{project_id}/domains_mapping</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p4901141485114"><a name="p4901141485114"></a><a name="p4901141485114"></a><a href="删除直播域名映射关系.md">删除直播域名映射关系</a></p>
</td>
</tr>
</tbody>
</table>

## 转码模板管理接口<a name="topic_live_04_overview_100015_section1490691275720"></a>

**表 2**  转码模板管理接口

<a name="topic_live_04_overview_100015_table182059123588"></a>
<table><thead align="left"><tr id="topic_live_04_overview_100015_row1520651265819"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="topic_live_04_overview_100015_p120881213585"><a name="topic_live_04_overview_100015_p120881213585"></a><a name="topic_live_04_overview_100015_p120881213585"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="topic_live_04_overview_100015_p520851285811"><a name="topic_live_04_overview_100015_p520851285811"></a><a name="topic_live_04_overview_100015_p520851285811"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="topic_live_04_overview_100015_row162091912185820"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p621119122585"><a name="topic_live_04_overview_100015_p621119122585"></a><a name="topic_live_04_overview_100015_p621119122585"></a>POST /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p32120125581"><a name="topic_live_04_overview_100015_p32120125581"></a><a name="topic_live_04_overview_100015_p32120125581"></a><a href="创建直播转码模板.md">创建直播转码模板</a></p>
</td>
</tr>
<tr id="row949921754913"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p521341265816"><a name="topic_live_04_overview_100015_p521341265816"></a><a name="topic_live_04_overview_100015_p521341265816"></a>DELETE /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p9215201235816"><a name="topic_live_04_overview_100015_p9215201235816"></a><a name="topic_live_04_overview_100015_p9215201235816"></a><a href="删除直播转码模板.md">删除直播转码模板</a></p>
</td>
</tr>
<tr id="row92461916298"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p18217171217581"><a name="topic_live_04_overview_100015_p18217171217581"></a><a name="topic_live_04_overview_100015_p18217171217581"></a>PUT /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p1721961215816"><a name="topic_live_04_overview_100015_p1721961215816"></a><a name="topic_live_04_overview_100015_p1721961215816"></a><a href="配置直播转码模板.md">配置直播转码模板</a></p>
</td>
</tr>
<tr id="topic_live_04_overview_100015_row11219121217581"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p9220141220583"><a name="topic_live_04_overview_100015_p9220141220583"></a><a name="topic_live_04_overview_100015_p9220141220583"></a>GET /v1/{project_id}/template/transcodings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p522101215584"><a name="topic_live_04_overview_100015_p522101215584"></a><a name="topic_live_04_overview_100015_p522101215584"></a><a href="查询直播转码模板.md">查询直播转码模板</a></p>
</td>
</tr>
</tbody>
</table>

## 流管理接口<a name="topic_live_04_overview_100015_section122718360575"></a>

**表 3**  流管理接口

<a name="topic_live_04_overview_100015_table082712210581"></a>
<table><thead align="left"><tr id="topic_live_04_overview_100015_row16829162285810"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="topic_live_04_overview_100015_p1183072218581"><a name="topic_live_04_overview_100015_p1183072218581"></a><a name="topic_live_04_overview_100015_p1183072218581"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="topic_live_04_overview_100015_p48311322205815"><a name="topic_live_04_overview_100015_p48311322205815"></a><a name="topic_live_04_overview_100015_p48311322205815"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4182162262819"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p9845722125818"><a name="topic_live_04_overview_100015_p9845722125818"></a><a name="topic_live_04_overview_100015_p9845722125818"></a>POST /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p18462226585"><a name="topic_live_04_overview_100015_p18462226585"></a><a name="topic_live_04_overview_100015_p18462226585"></a><a href="禁止直播推流.md">禁止直播推流</a></p>
</td>
</tr>
<tr id="row196644044911"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p98763498494"><a name="topic_live_04_overview_100015_p98763498494"></a><a name="topic_live_04_overview_100015_p98763498494"></a>GET /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p19876114904918"><a name="topic_live_04_overview_100015_p19876114904918"></a><a name="topic_live_04_overview_100015_p19876114904918"></a><a href="查询禁止直播推流列表.md">查询禁止直播推流列表</a></p>
</td>
</tr>
<tr id="row14261115914911"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p23041047172515"><a name="topic_live_04_overview_100015_p23041047172515"></a><a name="topic_live_04_overview_100015_p23041047172515"></a>DELETE /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p63041247182512"><a name="topic_live_04_overview_100015_p63041247182512"></a><a name="topic_live_04_overview_100015_p63041247182512"></a><a href="禁推恢复.md">禁推恢复</a></p>
</td>
</tr>
<tr id="topic_live_04_overview_100015_row1536853762513"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p16369337182517"><a name="topic_live_04_overview_100015_p16369337182517"></a><a name="topic_live_04_overview_100015_p16369337182517"></a>PUT /v1/{project_id}/stream/blocks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p83698370257"><a name="topic_live_04_overview_100015_p83698370257"></a><a name="topic_live_04_overview_100015_p83698370257"></a><a href="修改禁推属性.md">修改禁推属性</a></p>
</td>
</tr>
<tr id="row989524912176"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p689613491179"><a name="p689613491179"></a><a name="p689613491179"></a>GET /v1/{project_id}/realtime/streams</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p489620496175"><a name="p489620496175"></a><a name="p489620496175"></a><a href="查询直播中的流信息.md">查询直播中的流信息</a></p>
</td>
</tr>
</tbody>
</table>

## 日志管理接口<a name="section162381317182311"></a>

**表 4**  日志管理接口

<a name="table146921834132318"></a>
<table><thead align="left"><tr id="row66931345237"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p126931934102314"><a name="p126931934102314"></a><a name="p126931934102314"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p15693534152318"><a name="p15693534152318"></a><a name="p15693534152318"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2693113410238"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p16936349239"><a name="p16936349239"></a><a name="p16936349239"></a>GET /v1/{project_id}/logs</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p17693123462315"><a name="p17693123462315"></a><a name="p17693123462315"></a><a href="获取直播播放日志.md">获取直播播放日志</a></p>
</td>
</tr>
</tbody>
</table>

## 录制管理接口<a name="section38551539104716"></a>

**表 5**  录制管理接口

<a name="table17615951164714"></a>
<table><thead align="left"><tr id="row1461615119479"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p261675110472"><a name="p261675110472"></a><a name="p261675110472"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p1861655112477"><a name="p1861655112477"></a><a name="p1861655112477"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row16616125164710"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p461615114479"><a name="p461615114479"></a><a name="p461615114479"></a>POST /v1/{project_id}/record/rules</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p196161951134711"><a name="p196161951134711"></a><a name="p196161951134711"></a><a href="创建录制规则.md">创建录制规则</a></p>
</td>
</tr>
<tr id="row6616205112477"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p361625104717"><a name="p361625104717"></a><a name="p361625104717"></a>GET /v1/{project_id}/record/rules</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p161645154711"><a name="p161645154711"></a><a name="p161645154711"></a><a href="查询录制规则列表.md">查询录制规则列表</a></p>
</td>
</tr>
<tr id="row461619515477"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p7484154720494"><a name="p7484154720494"></a><a name="p7484154720494"></a>PUT /v1/{project_id}/record/rules/{id}</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1961618512477"><a name="p1961618512477"></a><a name="p1961618512477"></a><a href="修改录制规则.md">修改录制规则</a></p>
</td>
</tr>
<tr id="row20616195116470"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1898954711490"><a name="p1898954711490"></a><a name="p1898954711490"></a>DELETE /v1/{project_id}/record/rules/{id}</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1361635117471"><a name="p1361635117471"></a><a name="p1361635117471"></a><a href="删除录制规则.md">删除录制规则</a></p>
</td>
</tr>
<tr id="row1861635194710"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1444305364919"><a name="p1444305364919"></a><a name="p1444305364919"></a>GET /v1/{project_id}/record/rules/{id}</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p16616105115477"><a name="p16616105115477"></a><a name="p16616105115477"></a><a href="查询录制规则配置.md">查询录制规则配置</a></p>
</td>
</tr>
<tr id="row2027610359917"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p22764354913"><a name="p22764354913"></a><a name="p22764354913"></a>POST /v1/{project_id}/record/control</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p4276133510911"><a name="p4276133510911"></a><a name="p4276133510911"></a><a href="提交录制控制命令.md">提交录制控制命令</a></p>
</td>
</tr>
</tbody>
</table>

## 录制回调管理接口<a name="section138897110516"></a>

**表 6**  录制回调管理接口

<a name="table193661817165113"></a>
<table><thead align="left"><tr id="row11366111775120"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p1136611795114"><a name="p1136611795114"></a><a name="p1136611795114"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p1536691719511"><a name="p1536691719511"></a><a name="p1536691719511"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row12366131795115"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p9366101716514"><a name="p9366101716514"></a><a name="p9366101716514"></a>POST /v1/{project_id}/record/callbacks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1136691714518"><a name="p1136691714518"></a><a name="p1136691714518"></a><a href="创建录制回调配置.md">创建录制回调配置</a></p>
</td>
</tr>
<tr id="row20366817115110"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p11366171745114"><a name="p11366171745114"></a><a name="p11366171745114"></a>GET /v1/{project_id}/record/callbacks</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p7367121755118"><a name="p7367121755118"></a><a name="p7367121755118"></a><a href="查询录制回调配置列表.md">查询录制回调配置列表</a></p>
</td>
</tr>
<tr id="row5367121710511"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p83676171517"><a name="p83676171517"></a><a name="p83676171517"></a>PUT /v1/{project_id}/record/callbacks/{id}</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p936771713512"><a name="p936771713512"></a><a name="p936771713512"></a><a href="修改录制回调配置.md">修改录制回调配置</a></p>
</td>
</tr>
<tr id="row10367101765115"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1371661125512"><a name="p1371661125512"></a><a name="p1371661125512"></a>GET /v1/{project_id}/record/callbacks/{id}</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1473616109525"><a name="p1473616109525"></a><a name="p1473616109525"></a><a href="查询录制回调配置.md">查询录制回调配置</a></p>
</td>
</tr>
<tr id="row113677171512"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p2036717174518"><a name="p2036717174518"></a><a name="p2036717174518"></a>DELETE /v1/{project_id}/record/callbacks/{id}</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1136751719511"><a name="p1136751719511"></a><a name="p1136751719511"></a><a href="删除录制回调配置.md">删除录制回调配置</a></p>
</td>
</tr>
</tbody>
</table>

## 数据统计分析接口<a name="topic_live_04_overview_100015_section10546145517389"></a>

**表 7**  数据统计分析接口

<a name="topic_live_04_overview_100015_table7139143874320"></a>
<table><thead align="left"><tr id="topic_live_04_overview_100015_row121404387433"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="topic_live_04_overview_100015_p181401738204311"><a name="topic_live_04_overview_100015_p181401738204311"></a><a name="topic_live_04_overview_100015_p181401738204311"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="topic_live_04_overview_100015_p1914023884319"><a name="topic_live_04_overview_100015_p1914023884319"></a><a name="topic_live_04_overview_100015_p1914023884319"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="topic_live_04_overview_100015_row131406387435"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p41901144195219"><a name="p41901144195219"></a><a name="p41901144195219"></a>GET /v2/{project_id}/stats/bandwidth/detail</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1718212495527"><a name="p1718212495527"></a><a name="p1718212495527"></a><a href="查询播放带宽趋势接口.md">查询播放带宽趋势</a></p>
</td>
</tr>
<tr id="topic_live_04_overview_100015_row81401738204314"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p76968345533"><a name="p76968345533"></a><a name="p76968345533"></a>GET /v2/{project_id}/stats/traffic/detail</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p21402386439"><a name="topic_live_04_overview_100015_p21402386439"></a><a name="topic_live_04_overview_100015_p21402386439"></a><a href="查询播放流量趋势接口.md">查询播放流量趋势</a></p>
</td>
</tr>
<tr id="topic_live_04_overview_100015_row214043814430"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p12227328115315"><a name="p12227328115315"></a><a name="p12227328115315"></a>GET /v2/{project_id}/stats/bandwidth/peak</p>
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
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p58671473232"><a name="p58671473232"></a><a name="p58671473232"></a><a href="查询直播拉流HTTP状态码接口.md">查询直播拉流HTTP状态码</a></p>
</td>
</tr>
<tr id="row24551447204314"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p15455184794311"><a name="p15455184794311"></a><a name="p15455184794311"></a>GET /v2/{project_id}/stats/transcode</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1345534713437"><a name="p1345534713437"></a><a name="p1345534713437"></a><a href="查询转码用量接口.md">查询转码用量</a></p>
</td>
</tr>
<tr id="row1328522911371"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p137781353191414"><a name="p137781353191414"></a><a name="p137781353191414"></a>GET /v2/{project_id}/stats/record</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p162861129173713"><a name="p162861129173713"></a><a name="p162861129173713"></a><a href="查询录制用量接口.md">查询录制用量</a></p>
</td>
</tr>
<tr id="row737674715379"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p6629125310143"><a name="p6629125310143"></a><a name="p6629125310143"></a>GET /v2/{project_id}/stats/snapshot</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1937620476371"><a name="p1937620476371"></a><a name="p1937620476371"></a><a href="查询截图用量接口.md">查询截图用量</a></p>
</td>
</tr>
<tr id="row174991530436"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p139638597418"><a name="p139638597418"></a><a name="p139638597418"></a>GET /v2/{project_id}/stats/up-bandwidth/detail</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p2094953184410"><a name="p2094953184410"></a><a name="p2094953184410"></a><a href="查询上行带宽数据接口.md">查询上行带宽数据</a></p>
</td>
</tr>
<tr id="row8361135004316"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p8361750154319"><a name="p8361750154319"></a><a name="p8361750154319"></a>GET /v2/{project_id}/stats/stream-count</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1336114506438"><a name="p1336114506438"></a><a name="p1336114506438"></a><a href="查询域名维度推流路数接口.md">查询域名维度推流路数</a></p>
</td>
</tr>
<tr id="row79814964413"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p59864916446"><a name="p59864916446"></a><a name="p59864916446"></a>GET /v2/{project_id}/stats/history/streams</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p398149174419"><a name="p398149174419"></a><a name="p398149174419"></a><a href="查询历史推流列表接口.md">查询历史推流列表</a></p>
</td>
</tr>
<tr id="row3721174311343"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p37221543103415"><a name="p37221543103415"></a><a name="p37221543103415"></a>GET /v2/{project_id}/stats/stream-portraits</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p5722204333410"><a name="p5722204333410"></a><a name="p5722204333410"></a><a href="查询播放画像信息接口.md">查询播放画像信息</a></p>
</td>
</tr>
</tbody>
</table>

## 流监控接口<a name="topic_live_04_overview_100015_section186134919393"></a>

**表 8**  流监控接口

<a name="topic_live_04_overview_100015_table58515224617"></a>
<table><thead align="left"><tr id="topic_live_04_overview_100015_row148782164610"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="topic_live_04_overview_100015_p2087182124620"><a name="topic_live_04_overview_100015_p2087182124620"></a><a name="topic_live_04_overview_100015_p2087182124620"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="topic_live_04_overview_100015_p087329465"><a name="topic_live_04_overview_100015_p087329465"></a><a name="topic_live_04_overview_100015_p087329465"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="topic_live_04_overview_100015_row5877214464"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p135861757195313"><a name="p135861757195313"></a><a name="p135861757195313"></a>GET /v2/{project_id}/stats/stream/framerate</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p528794365311"><a name="p528794365311"></a><a name="p528794365311"></a><a href="查询推流帧率数据接口.md">查询推流帧率数据</a></p>
</td>
</tr>
<tr id="topic_live_04_overview_100015_row1087228461"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p15600520545"><a name="p15600520545"></a><a name="p15600520545"></a>GET /v2/{project_id}/stats/stream/bitrate</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p10638165125319"><a name="p10638165125319"></a><a name="p10638165125319"></a><a href="查询推流码率数据接口.md">查询推流码率数据</a></p>
</td>
</tr>
</tbody>
</table>

## 流管理历史接口<a name="section468132819420"></a>

**表 9**  流管理历史接口

<a name="table990413465435"></a>
<table><thead align="left"><tr id="row17904124618439"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p1590484644319"><a name="p1590484644319"></a><a name="p1590484644319"></a>接口</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p1890464694316"><a name="p1890464694316"></a><a name="p1890464694316"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row99044469439"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p1485452214582"><a name="topic_live_04_overview_100015_p1485452214582"></a><a name="topic_live_04_overview_100015_p1485452214582"></a>GET /v1/{project_id}/stream/bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p158553227588"><a name="topic_live_04_overview_100015_p158553227588"></a><a name="topic_live_04_overview_100015_p158553227588"></a><a href="查询直播加速的带宽数据.md">查询直播加速的带宽数据</a></p>
</td>
</tr>
<tr id="row6904184618437"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p8857132211584"><a name="topic_live_04_overview_100015_p8857132211584"></a><a name="topic_live_04_overview_100015_p8857132211584"></a>GET /v1/{project_id}/stream/traffic</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p138581422195812"><a name="topic_live_04_overview_100015_p138581422195812"></a><a name="topic_live_04_overview_100015_p138581422195812"></a><a href="查询直播加速的流量数据.md">查询直播加速的流量数据</a></p>
</td>
</tr>
<tr id="row9904144617435"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="topic_live_04_overview_100015_p38582022135817"><a name="topic_live_04_overview_100015_p38582022135817"></a><a name="topic_live_04_overview_100015_p38582022135817"></a>GET /v1/{project_id}/stream/users</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="topic_live_04_overview_100015_p1886019228586"><a name="topic_live_04_overview_100015_p1886019228586"></a><a name="topic_live_04_overview_100015_p1886019228586"></a><a href="查询直播播放在线人数.md">查询直播播放在线人数</a></p>
</td>
</tr>
</tbody>
</table>

## 录制至VOD接口<a name="section6534185517572"></a>

**表 10**  录制至VOD接口

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
<tr id="row52731527145615"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p53317710573"><a name="p53317710573"></a><a name="p53317710573"></a>DELETE /v1/{project_id}/record/config</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p13316716571"><a name="p13316716571"></a><a name="p13316716571"></a><a href="删除录制配置.md">删除录制配置</a></p>
</td>
</tr>
<tr id="row1331775573"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1933197115719"><a name="p1933197115719"></a><a name="p1933197115719"></a>GET /v1/{project_id}/record/config</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1133873574"><a name="p1133873574"></a><a name="p1133873574"></a><a href="查询录制配置.md">查询录制配置</a></p>
</td>
</tr>
</tbody>
</table>

