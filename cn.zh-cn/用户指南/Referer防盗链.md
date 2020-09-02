# Referer防盗链<a name="live_01_0048"></a>

Referer防盗链功能是基于HTTP协议支持的Referer机制，通过播放请求中携带的Referer字段识别请求来源。配置Referer黑名单或白名单后，CDN会根据名单对请求来源进行过滤，允许或拒绝播放请求。

## 注意事项<a name="zh-cn_topic_0194695754_section9354115514113"></a>

-   该功能为可选项，默认不启用。
-   Referer黑名单与Referer白名单互斥，不支持同时设置。
-   黑名单或白名单中的域名最多支持配置100条。
-   黑名单或白名单中配置的域名为正则匹配。如填写“^http://test.\*com$“，则“http://test.example.com“和“http://test.example01.com“也会匹配成功。

## 前提条件<a name="section38573451572"></a>

-   已[添加推流域名和播放域名](添加域名.md)，且已完成[域名关联](关联域名.md)。
-   已在域名DNS服务商处完成[CNAME解析配置](配置CNAME.md)。

## 操作步骤<a name="zh-cn_topic_0194695754_section12744193714437"></a>

1.  登录[视频直播控制台](https://console.huaweicloud.com/live)。
2.  在左侧导航树中选择“域名管理“，进入域名管理页面。
3.  在需要配置鉴权信息的播放域名行单击“管理“。
4.  在左侧导航树中选择“基础配置 \> 鉴权配置“。
5.  选择“Referer防盗链“，弹出“Referer防盗链“对话框。
6.  单击“开关“，配置Referer防盗链参数，如[图1](#zh-cn_topic_0194695754_fig657733201016)所示。

    **图 1**  配置Referer防盗链<a name="zh-cn_topic_0194695754_fig657733201016"></a>  
    ![](figures/配置Referer防盗链.png "配置Referer防盗链")

    防盗链配置及对应访问权限说明如[表1](#zh-cn_topic_0194695754_zh-cn_topic_0129356805_table837817528191)所示。

    **表 1**  Referer防盗链配置

    <a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_table837817528191"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_row19890101885714"><th class="cellrowborder" valign="top" width="20.03%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p182343561940"><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p182343561940"></a><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p182343561940"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="79.97%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p6890181895711"><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p6890181895711"></a><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p6890181895711"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_row1089016185579"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p323410562417"><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p323410562417"></a><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p323410562417"></a>类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.97%" headers="mcps1.2.3.1.2 "><div class="p" id="zh-cn_topic_0194695754_p4796204561519"><a name="zh-cn_topic_0194695754_p4796204561519"></a><a name="zh-cn_topic_0194695754_p4796204561519"></a>支持黑名单和白名单模式。<a name="zh-cn_topic_0194695754_ul1528259181510"></a><a name="zh-cn_topic_0194695754_ul1528259181510"></a><ul id="zh-cn_topic_0194695754_ul1528259181510"><li>Referer黑名单：允许非名单内的域名请求访问资源，拒绝名单中的域名请求访问。</li><li>Referer白名单：允许名单内的域名请求访问资源，拒绝其它域名请求访问。</li></ul>
    </div>
    <p id="zh-cn_topic_0194695754_p030612381510"><a name="zh-cn_topic_0194695754_p030612381510"></a><a name="zh-cn_topic_0194695754_p030612381510"></a>您可以设置是否允许空Referer字段访问资源，即是否允许通过浏览器地址栏直接访问资源URL。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_row4725335657"><td class="cellrowborder" valign="top" width="20.03%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p1872653520517"><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p1872653520517"></a><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p1872653520517"></a>规则</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.97%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p15426936145216"><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p15426936145216"></a><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_zh-cn_topic_0111450891_p15426936145216"></a>黑名单或白名单中的域名。</p>
    <a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_ul1316151174219"></a><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_ul1316151174219"></a><ul id="zh-cn_topic_0194695754_zh-cn_topic_0129356805_ul1316151174219"><li>规则最多支持100条（最少1条），每一行一条记录，或者以英文<span class="parmvalue" id="zh-cn_topic_0194695754_zh-cn_topic_0129356805_parmvalue1116131117425"><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_parmvalue1116131117425"></a><a name="zh-cn_topic_0194695754_zh-cn_topic_0129356805_parmvalue1116131117425"></a>“;”</span>分隔。</li><li>域名为正则匹配，若填写<span class="parmvalue" id="parmvalue171721618913"><a name="parmvalue171721618913"></a><a name="parmvalue171721618913"></a>“^http://test.*com$”</span>，则<span class="parmvalue" id="parmvalue47171616297"><a name="parmvalue47171616297"></a><a name="parmvalue47171616297"></a>“http://test.example.com”</span>和<span class="parmvalue" id="parmvalue1371721613914"><a name="parmvalue1371721613914"></a><a name="parmvalue1371721613914"></a>“http://test.example01.com”</span>也会匹配成功。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

7.  配置完成后，单击“确定“。

