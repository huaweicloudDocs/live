# 查询直播拉流HTTP状态码接口<a name="ListQueryHttpCode"></a>

## 功能介绍<a name="section510817425363"></a>

查询直播拉流HTTP状态码接口。 获取加速域名1分钟粒度的HTTP返回码。

最大查询跨度不能超过24小时，最大查询周期7天。

## 调试<a name="section1510817426368"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=Live&api=ListQueryHttpCode)中调试该接口。

## URI<a name="section410814429362"></a>

GET /v2/\{project\_id\}/stats/httpcodes

**表 1**  路径参数

<a name="table21091642133616"></a>
<table><thead align="left"><tr id="row4109542123617"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p310910420366"><a name="p310910420366"></a><a name="p310910420366"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p4109124211361"><a name="p4109124211361"></a><a name="p4109124211361"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p12110442113617"><a name="p12110442113617"></a><a name="p12110442113617"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p16110142143615"><a name="p16110142143615"></a><a name="p16110142143615"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row18109104253617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p81106421364"><a name="p81106421364"></a><a name="p81106421364"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p1511074210366"><a name="p1511074210366"></a><a name="p1511074210366"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p21101442113611"><a name="p21101442113611"></a><a name="p21101442113611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p9111542143610"><a name="p9111542143610"></a><a name="p9111542143610"></a>项目ID，获取方法请参考<a href="https://support.huaweicloud.com/api-live/live_03_0023.html" target="_blank" rel="noopener noreferrer">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Query参数

<a name="table811144293610"></a>
<table><thead align="left"><tr id="row61118423366"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p911211428367"><a name="p911211428367"></a><a name="p911211428367"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p131121642173610"><a name="p131121642173610"></a><a name="p131121642173610"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p11121942143611"><a name="p11121942143611"></a><a name="p11121942143611"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p18112124253610"><a name="p18112124253610"></a><a name="p18112124253610"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row191116422367"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p51121342123612"><a name="p51121342123612"></a><a name="p51121342123612"></a>play_domains</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p19112164214367"><a name="p19112164214367"></a><a name="p19112164214367"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p17113174211369"><a name="p17113174211369"></a><a name="p17113174211369"></a>ARRAY</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p1113144233619"><a name="p1113144233619"></a><a name="p1113144233619"></a>播放域名列表，最多支持查询10个域名，多个域名以逗号分隔。</p>
</td>
</tr>
<tr id="row1411184293611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p711324214367"><a name="p711324214367"></a><a name="p711324214367"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p11138423361"><a name="p11138423361"></a><a name="p11138423361"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p51136423363"><a name="p51136423363"></a><a name="p51136423363"></a>ARRAY</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p111135425367"><a name="p111135425367"></a><a name="p111135425367"></a>状态码。</p>
</td>
</tr>
<tr id="row19111542113613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1811444210367"><a name="p1811444210367"></a><a name="p1811444210367"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p1211414253617"><a name="p1211414253617"></a><a name="p1211414253617"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p16114194212360"><a name="p16114194212360"></a><a name="p16114194212360"></a>ARRAY</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p19114144293618"><a name="p19114144293618"></a><a name="p19114144293618"></a>区域列表。具体取值请参考<a href="省份名称缩写.md">省份名称缩写</a>，不填写查询所有区域。</p>
</td>
</tr>
<tr id="row411124211365"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13114134210364"><a name="p13114134210364"></a><a name="p13114134210364"></a>isp</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p011415425364"><a name="p011415425364"></a><a name="p011415425364"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1511513424367"><a name="p1511513424367"></a><a name="p1511513424367"></a>ARRAY</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p61151242193614"><a name="p61151242193614"></a><a name="p61151242193614"></a>运营商列表，取值如下：</p>
<a name="ul1911564210366"></a><a name="ul1911564210366"></a><ul id="ul1911564210366"><li>"CMCC ：移动"</li><li>"CTCC ： 电信"</li><li>"CUCC ：联通"</li><li>"OTHER: 其他"</li></ul>
<p id="p2115842123618"><a name="p2115842123618"></a><a name="p2115842123618"></a>不填写查询所有运营商。</p>
</td>
</tr>
<tr id="row16111642113612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p4115134253614"><a name="p4115134253614"></a><a name="p4115134253614"></a>start_time</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p16116164263620"><a name="p16116164263620"></a><a name="p16116164263620"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p18116194213363"><a name="p18116194213363"></a><a name="p18116194213363"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p3116842193613"><a name="p3116842193613"></a><a name="p3116842193613"></a>起始时间。日期格式按照ISO8601表示法，并使用UTC时间。</p>
<p id="p411619424365"><a name="p411619424365"></a><a name="p411619424365"></a>格式为：YYYY-MM-DDThh:mm:ssZ。若参数为空，默认查询最近1小时数据。</p>
<p id="p3116164273610"><a name="p3116164273610"></a><a name="p3116164273610"></a>最大查询跨度1天，最大查询周期7天。</p>
</td>
</tr>
<tr id="row13111124213361"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p61161942123612"><a name="p61161942123612"></a><a name="p61161942123612"></a>end_time</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p121169421361"><a name="p121169421361"></a><a name="p121169421361"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p121178425366"><a name="p121178425366"></a><a name="p121178425366"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p7117114211362"><a name="p7117114211362"></a><a name="p7117114211362"></a>结束时间。日期格式按照ISO8601表示法，并使用UTC时间。</p>
<p id="p18117114210361"><a name="p18117114210361"></a><a name="p18117114210361"></a>格式为：YYYY-MM-DDThh:mm:ssZ。</p>
<p id="p81172428367"><a name="p81172428367"></a><a name="p81172428367"></a>若参数为空，默认为当前时间。结束时间需大于起始时间。</p>
<p id="p21172425369"><a name="p21172425369"></a><a name="p21172425369"></a>最大查询跨度1天，最大查询周期7天。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section711724215367"></a>

**表 3**  请求Header参数

<a name="HeaderParameter"></a>
<table><thead align="left"><tr id="row1411734263615"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p11181042163618"><a name="p11181042163618"></a><a name="p11181042163618"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p31182425369"><a name="p31182425369"></a><a name="p31182425369"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p311824213361"><a name="p311824213361"></a><a name="p311824213361"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p11187428364"><a name="p11187428364"></a><a name="p11187428364"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1011854215362"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p111914273613"><a name="p111914273613"></a><a name="p111914273613"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p11119114203612"><a name="p11119114203612"></a><a name="p11119114203612"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p151196426363"><a name="p151196426363"></a><a name="p151196426363"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p01191142133610"><a name="p01191142133610"></a><a name="p01191142133610"></a>用户Token。使用Token鉴权方式时必选。 通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）。</p>
</td>
</tr>
<tr id="row1611819427366"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p14119042203613"><a name="p14119042203613"></a><a name="p14119042203613"></a>Authorization</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p61192042133615"><a name="p61192042133615"></a><a name="p61192042133615"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p171191242113614"><a name="p171191242113614"></a><a name="p171191242113614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p412024220368"><a name="p412024220368"></a><a name="p412024220368"></a>使用AK/SK方式认证时必选，携带的鉴权信息。</p>
</td>
</tr>
<tr id="row811814426369"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p41201842133617"><a name="p41201842133617"></a><a name="p41201842133617"></a>X-Sdk-Date</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p91206427363"><a name="p91206427363"></a><a name="p91206427363"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1912094233619"><a name="p1912094233619"></a><a name="p1912094233619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p612015424368"><a name="p612015424368"></a><a name="p612015424368"></a>使用AK/SK方式认证时必选，请求的发生时间。</p>
</td>
</tr>
<tr id="row1411819422360"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p412094216361"><a name="p412094216361"></a><a name="p412094216361"></a>X-Project-Id</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p91211542103618"><a name="p91211542103618"></a><a name="p91211542103618"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14121042133615"><a name="p14121042133615"></a><a name="p14121042133615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p13121174219363"><a name="p13121174219363"></a><a name="p13121174219363"></a>使用AK/SK方式认证时必选，携带项目ID信息, 与路径参数中的项目ID相同。</p>
</td>
</tr>
</tbody>
</table>

## 响应参数<a name="section112111422364"></a>

**状态码为 200 时:**

**表 4**  响应Header参数

<a name="ResponseHeaderParameter"></a>
<table><thead align="left"><tr id="row1912215429364"><th class="cellrowborder" valign="top" width="30%" id="mcps1.2.4.1.1"><p id="p512244293611"><a name="p512244293611"></a><a name="p512244293611"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p10122642193615"><a name="p10122642193615"></a><a name="p10122642193615"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="p16122184212364"><a name="p16122184212364"></a><a name="p16122184212364"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row41227420369"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.4.1.1 "><p id="p31231942173612"><a name="p31231942173612"></a><a name="p31231942173612"></a>X-request-id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51238421363"><a name="p51238421363"></a><a name="p51238421363"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p161231042163611"><a name="p161231042163611"></a><a name="p161231042163611"></a>请求的唯一标识</p>
</td>
</tr>
</tbody>
</table>

**表 5**  响应Body参数

<a name="responseParameter"></a>
<table><thead align="left"><tr id="row612354253616"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p9124342163612"><a name="p9124342163612"></a><a name="p9124342163612"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p11124194216362"><a name="p11124194216362"></a><a name="p11124194216362"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p19124194216364"><a name="p19124194216364"></a><a name="p19124194216364"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row6123134263616"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1912411422362"><a name="p1912411422362"></a><a name="p1912411422362"></a>data_series</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p112417422368"><a name="p112417422368"></a><a name="p112417422368"></a>Array of <a href="#response_HttpCodeSummary">HttpCodeSummary</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p412474216367"><a name="p412474216367"></a><a name="p412474216367"></a>基于时间轴的状态码</p>
</td>
</tr>
</tbody>
</table>

**表 6**  HttpCodeSummary

<a name="response_HttpCodeSummary"></a>
<table><thead align="left"><tr id="row812574233616"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p20125154212366"><a name="p20125154212366"></a><a name="p20125154212366"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p112554215364"><a name="p112554215364"></a><a name="p112554215364"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p6126342133614"><a name="p6126342133614"></a><a name="p6126342133614"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row14125144213361"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p161261042133615"><a name="p161261042133615"></a><a name="p161261042133615"></a>http_codes</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1012618424366"><a name="p1012618424366"></a><a name="p1012618424366"></a>Array of <a href="#response_HttpCode">HttpCode</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10126194203615"><a name="p10126194203615"></a><a name="p10126194203615"></a>状态码信息</p>
</td>
</tr>
<tr id="row131251742113618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1012611427362"><a name="p1012611427362"></a><a name="p1012611427362"></a>time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1512612429365"><a name="p1512612429365"></a><a name="p1512612429365"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2126164283618"><a name="p2126164283618"></a><a name="p2126164283618"></a>采样时间。日期格式按照ISO8601表示法，并使用UTC时间。 格式为：YYYY-MM-DDThh:mm:ssZ 。</p>
</td>
</tr>
</tbody>
</table>

**表 7**  HttpCode

<a name="response_HttpCode"></a>
<table><thead align="left"><tr id="row181271042153613"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1312715423365"><a name="p1312715423365"></a><a name="p1312715423365"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p4127124293615"><a name="p4127124293615"></a><a name="p4127124293615"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p131281742173614"><a name="p131281742173614"></a><a name="p131281742173614"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1312744212369"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4128642163610"><a name="p4128642163610"></a><a name="p4128642163610"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2012834273611"><a name="p2012834273611"></a><a name="p2012834273611"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p512819422367"><a name="p512819422367"></a><a name="p512819422367"></a>状态码</p>
</td>
</tr>
<tr id="row9127124212369"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7128124273614"><a name="p7128124273614"></a><a name="p7128124273614"></a>count</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1112811422368"><a name="p1112811422368"></a><a name="p1112811422368"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18128134213366"><a name="p18128134213366"></a><a name="p18128134213366"></a>状态码出现次数</p>
</td>
</tr>
<tr id="row121271942173618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4129134293617"><a name="p4129134293617"></a><a name="p4129134293617"></a>proportion</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p31291342133610"><a name="p31291342133610"></a><a name="p31291342133610"></a>Double</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15129184273615"><a name="p15129184273615"></a><a name="p15129184273615"></a>状态码在对应时间点中的占比，保留4位小数。</p>
</td>
</tr>
</tbody>
</table>

**状态码为 400 时:**

**表 8**  响应Header参数

<a name="table11129134214367"></a>
<table><thead align="left"><tr id="row13129154233618"><th class="cellrowborder" valign="top" width="30%" id="mcps1.2.4.1.1"><p id="p813034211365"><a name="p813034211365"></a><a name="p813034211365"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p161301242113617"><a name="p161301242113617"></a><a name="p161301242113617"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="p17130242183614"><a name="p17130242183614"></a><a name="p17130242183614"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row111290426361"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.4.1.1 "><p id="p1713010421361"><a name="p1713010421361"></a><a name="p1713010421361"></a>X-request-id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11130144233615"><a name="p11130144233615"></a><a name="p11130144233615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p51308423364"><a name="p51308423364"></a><a name="p51308423364"></a>请求的唯一标识</p>
</td>
</tr>
</tbody>
</table>

**表 9**  响应Body参数

<a name="table8131144214364"></a>
<table><thead align="left"><tr id="row2131942143610"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p19131104223613"><a name="p19131104223613"></a><a name="p19131104223613"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p6131194253616"><a name="p6131194253616"></a><a name="p6131194253616"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1213294253614"><a name="p1213294253614"></a><a name="p1213294253614"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row151311429369"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16132642113610"><a name="p16132642113610"></a><a name="p16132642113610"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12132442153613"><a name="p12132442153613"></a><a name="p12132442153613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17132104210364"><a name="p17132104210364"></a><a name="p17132104210364"></a>错误码。</p>
</td>
</tr>
<tr id="row9131164214369"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1213234213612"><a name="p1213234213612"></a><a name="p1213234213612"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p141333427369"><a name="p141333427369"></a><a name="p141333427369"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13133134233610"><a name="p13133134233610"></a><a name="p13133134233610"></a>错误描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section151331242103617"></a>

```
GET /v2/{project_id}/stats/httpcode?play_domains=example.huawei.com,example1.huawei.com&start_time=2020-07-23T07:00:00Z&end_time=2020-07-23T08:00:00Z

```

## 响应示例<a name="section5133184212361"></a>

**状态码为 200 时:**

处理成功返回。

```
{
  "data_series" : [ {
    "time" : "2020-06-04T07:00:00Z",
    "http_codes" : [ {
      "code" : 200,
      "count" : 750,
      "proportion" : 0.5211
    }, {
      "code" : 400,
      "count" : 650,
      "proportion" : 0.4789
    } ]
  }, {
    "time" : "2020-06-04T07:01:00Z",
    "http_codes" : [ {
      "code" : 200,
      "count" : 1000,
      "proportion" : 1
    }, {
      "code" : 400,
      "count" : 0,
      "proportion" : 0
    } ]
  } ]
}
```

**状态码为 400 时:**

参数错误。

```
{
  "error_code" : "LIVE.100011001",
  "error_msg" : "请求参数非法：play_domains。"
}
```

## 状态码<a name="section8137642103618"></a>

<a name="table6250"></a>
<table><thead align="left"><tr id="row1137204217364"><th class="cellrowborder" valign="top" width="15%" id="mcps1.1.3.1.1"><p id="p1413824212367"><a name="p1413824212367"></a><a name="p1413824212367"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="85%" id="mcps1.1.3.1.2"><p id="p1138154223615"><a name="p1138154223615"></a><a name="p1138154223615"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1213774293613"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p9138114216369"><a name="p9138114216369"></a><a name="p9138114216369"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1013894213610"><a name="p1013894213610"></a><a name="p1013894213610"></a>处理成功返回。</p>
</td>
</tr>
<tr id="row131371942163611"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.3.1.1 "><p id="p4138104293617"><a name="p4138104293617"></a><a name="p4138104293617"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="85%" headers="mcps1.1.3.1.2 "><p id="p1813824210362"><a name="p1813824210362"></a><a name="p1813824210362"></a>参数错误。</p>
</td>
</tr>
</tbody>
</table>

## 错误码<a name="section913974211362"></a>

请参见[错误码](错误码.md)。

