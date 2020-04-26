# Key防盗链<a name="live01000302"></a>

为保障直播资源不被非法盗用，您可以使用直播的Key防盗链功能，在原始推流或播放地址末尾加上鉴权信息。在主播请求直播推流或观众请求播放时，CDN会对其URL带的加密信息进行合法性判断，仅校验通过的请求会予以响应，其它非法的访问将予以拒绝。

## 工作原理<a name="section762512381161"></a>

**图 1**  Key防盗链工作原理<a name="fig139571941829"></a>  
![](figures/Key防盗链工作原理.png "Key防盗链工作原理")

流程说明如下所示：

1.  租户在直播控制台开启Key防盗链功能，并配置Key值和时长。
2.  直播服务将租户配置Key值和时长下发到CDN节点中。
3.  主播/观众通过租户提供的鉴权推流/播放URL向CDN请求推流或播放。
4.  CDN根据推流或播放URL中携带的鉴权信息校验请求的合法性，仅校验通过的请求会被允许。

## 注意事项<a name="section257818139314"></a>

-   该功能为可选项，默认不启用。
-   启用该功能后，原始直播加速URL将无法使用，需要按规则生成合法的防盗链URL。
-   若防盗链URL过期，或者签名不能通过，直播流将播放失败，并返回“403 Forbidden”信息。
-   若需要关闭Key防盗链，请[提交工单](https://console.huaweicloud.com/ticket/?#/ticketindex/business?productTypeId=ffb4ebf5fb094bc6aef0129c276ce42e)申请。

## 开启Key防盗链<a name="section11844175984418"></a>

1.  登录[视频直播控制台](https://console.huaweicloud.com/live)。
2.  在左侧导航树中选择“域名管理“，进入域名管理页面。
3.  在需要配置鉴权信息的播放域名行右侧单击“管理“。
4.  <a name="li17393202514236"></a>在左侧导航树中选择“基础配置 \> 鉴权配置 \> Key防盗链“。在弹出的页面中打“开关”，并配置Key防盗链参数。

    **图 2**  配置Key防盗链<a name="fig72428511927"></a>  
    ![](figures/配置Key防盗链.png "配置Key防盗链")

    -   **Key**：鉴权key值，支持自定义设置，由16位的大小写字母和数字组成。
    -   **时长**：URL鉴权信息的超时时长，指的是鉴权信息中携带的请求时间与直播服务收到请求时的时间的最大差值，用于检查直播推流URL或者直播播放URL是否已过期，单位：秒，范围限制：1分钟-30天。

5.  配置完成后，单击“确定“。
6.  [提交工单](https://console.huaweicloud.com/ticket/?#/ticketindex/business?productTypeId=ffb4ebf5fb094bc6aef0129c276ce42e)申请Key防盗链配置审核。

    若您修改了Key防盗链相关参数，也需要[提交工单](https://console.huaweicloud.com/ticket/?#/ticketindex/business?productTypeId=ffb4ebf5fb094bc6aef0129c276ce42e)重新审核，提交工单时，需要提交的信息如[表1](#table204411582162)所示。

    **表 1**  Key防盗链配置审核

    <a name="table204411582162"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0176508927_row3705145215912"><th class="cellrowborder" valign="top" width="35.8%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0176508927_p10705352105920"><a name="zh-cn_topic_0176508927_p10705352105920"></a><a name="zh-cn_topic_0176508927_p10705352105920"></a>信息</p>
    </th>
    <th class="cellrowborder" valign="top" width="64.2%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0176508927_p187057529593"><a name="zh-cn_topic_0176508927_p187057529593"></a><a name="zh-cn_topic_0176508927_p187057529593"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0176508927_row13706125235912"><td class="cellrowborder" valign="top" width="35.8%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0176508927_p67061452105919"><a name="zh-cn_topic_0176508927_p67061452105919"></a><a name="zh-cn_topic_0176508927_p67061452105919"></a>推流域名</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.2%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0176508927_p98521845113"><a name="zh-cn_topic_0176508927_p98521845113"></a><a name="zh-cn_topic_0176508927_p98521845113"></a>需要配置Key防盗链的直播推流域名。</p>
    <p id="zh-cn_topic_0176508927_p283722417117"><a name="zh-cn_topic_0176508927_p283722417117"></a><a name="zh-cn_topic_0176508927_p283722417117"></a>示例：test-push.example.com</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0176508927_row127061952185917"><td class="cellrowborder" valign="top" width="35.8%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0176508927_p137061752135918"><a name="zh-cn_topic_0176508927_p137061752135918"></a><a name="zh-cn_topic_0176508927_p137061752135918"></a>播放域名</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.2%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0176508927_p5643957184413"><a name="zh-cn_topic_0176508927_p5643957184413"></a><a name="zh-cn_topic_0176508927_p5643957184413"></a>需要配置Key防盗链的直播播放域名。</p>
    <p id="zh-cn_topic_0176508927_p135771000512"><a name="zh-cn_topic_0176508927_p135771000512"></a><a name="zh-cn_topic_0176508927_p135771000512"></a>示例：test-play.example.com</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0176508927_row1970635214595"><td class="cellrowborder" valign="top" width="35.8%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0176508927_p14706155217595"><a name="zh-cn_topic_0176508927_p14706155217595"></a><a name="zh-cn_topic_0176508927_p14706155217595"></a>Key值</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.2%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0176508927_p570619523595"><a name="zh-cn_topic_0176508927_p570619523595"></a><a name="zh-cn_topic_0176508927_p570619523595"></a>请填写为<a href="#li17393202514236">4</a>中设置的Key值。</p>
    <p id="zh-cn_topic_0176508927_p1970213424528"><a name="zh-cn_topic_0176508927_p1970213424528"></a><a name="zh-cn_topic_0176508927_p1970213424528"></a>示例：9wAynnEtvouJwJMs</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0176508927_row124041522164413"><td class="cellrowborder" valign="top" width="35.8%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0176508927_p144055227441"><a name="zh-cn_topic_0176508927_p144055227441"></a><a name="zh-cn_topic_0176508927_p144055227441"></a>时长</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.2%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0176508927_p194051922104410"><a name="zh-cn_topic_0176508927_p194051922104410"></a><a name="zh-cn_topic_0176508927_p194051922104410"></a>请填写为<a href="#li17393202514236">4</a>中设置的时长。</p>
    <p id="zh-cn_topic_0176508927_p9162145714545"><a name="zh-cn_topic_0176508927_p9162145714545"></a><a name="zh-cn_topic_0176508927_p9162145714545"></a>示例：120</p>
    </td>
    </tr>
    </tbody>
    </table>

    审核通过后，您才可以通过鉴权URL进行推流或播放。请参见[生成鉴权URL](#section179511631145218)获取携带鉴权信息的推流和播放地址。


## 生成鉴权URL<a name="section179511631145218"></a>

鉴权URL的组成如下所示：

```
原始地址?auth_info=加密串.EncodedIV
```

鉴权字段的生成算法如下所示：

-   **LiveID**=<AppName\>+"/"+<StreamName\>
-   **加密串**=UrlEncode\(Base64\(AES128\(<Key\>,"$"+<Timestamp\>+"$"+<LiveID\>+"$"+<CheckLevel\>\)\)\)
-   **EncodedIV**=Hex\(加密使用的IV\)

算法中各加密参数说明如[表2](#table542713310247)所示。

**表 2**  加密参数说明

<a name="table542713310247"></a>
<table><thead align="left"><tr id="row7427193314245"><th class="cellrowborder" valign="top" width="25.1%" id="mcps1.2.3.1.1"><p id="p54275331249"><a name="p54275331249"></a><a name="p54275331249"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="74.9%" id="mcps1.2.3.1.2"><p id="p1942783313245"><a name="p1942783313245"></a><a name="p1942783313245"></a>参数说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18247112672719"><td class="cellrowborder" valign="top" width="25.1%" headers="mcps1.2.3.1.1 "><p id="p724892632711"><a name="p724892632711"></a><a name="p724892632711"></a>AppName</p>
</td>
<td class="cellrowborder" valign="top" width="74.9%" headers="mcps1.2.3.1.2 "><p id="p19248226172715"><a name="p19248226172715"></a><a name="p19248226172715"></a>应用名称，与推流或播放地址中的AppName一致。</p>
</td>
</tr>
<tr id="row18828643142815"><td class="cellrowborder" valign="top" width="25.1%" headers="mcps1.2.3.1.1 "><p id="p1582915435282"><a name="p1582915435282"></a><a name="p1582915435282"></a>StreamName</p>
</td>
<td class="cellrowborder" valign="top" width="74.9%" headers="mcps1.2.3.1.2 "><p id="p982918435288"><a name="p982918435288"></a><a name="p982918435288"></a>流名称，与推流或播放地址中的StreamName一致。</p>
</td>
</tr>
<tr id="row1652817233815"><td class="cellrowborder" valign="top" width="25.1%" headers="mcps1.2.3.1.1 "><p id="p45297233818"><a name="p45297233818"></a><a name="p45297233818"></a>Key</p>
</td>
<td class="cellrowborder" valign="top" width="74.9%" headers="mcps1.2.3.1.2 "><p id="p14529132133816"><a name="p14529132133816"></a><a name="p14529132133816"></a>鉴权Key值，<a href="#section11844175984418">开启Key防盗链</a>中配置的Key值。</p>
</td>
</tr>
<tr id="row343529172915"><td class="cellrowborder" valign="top" width="25.1%" headers="mcps1.2.3.1.1 "><p id="p342723310248"><a name="p342723310248"></a><a name="p342723310248"></a>LiveID</p>
</td>
<td class="cellrowborder" valign="top" width="74.9%" headers="mcps1.2.3.1.2 "><p id="p10427173320240"><a name="p10427173320240"></a><a name="p10427173320240"></a>直播流ID，用于标识唯一的直播流，由AppName和StreamName组成。</p>
<p id="p314954318210"><a name="p314954318210"></a><a name="p314954318210"></a>LiveID=&lt;AppName&gt;+"/"+&lt;StreamName&gt;</p>
</td>
</tr>
<tr id="row20427103317248"><td class="cellrowborder" valign="top" width="25.1%" headers="mcps1.2.3.1.1 "><p id="p132630132713"><a name="p132630132713"></a><a name="p132630132713"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="74.9%" headers="mcps1.2.3.1.2 "><p id="p5427203342412"><a name="p5427203342412"></a><a name="p5427203342412"></a>鉴权参数生成的UTC时间，格式为<span class="parmvalue" id="parmvalue13356183910354"><a name="parmvalue13356183910354"></a><a name="parmvalue13356183910354"></a>“yyyyMMddHHmmss”</span>，用于检查鉴权参数是否已过期，即Timestamp和当前时间差值的绝对值是否大于配置的超时时长。</p>
</td>
</tr>
<tr id="row134274335245"><td class="cellrowborder" valign="top" width="25.1%" headers="mcps1.2.3.1.1 "><p id="p1642715335241"><a name="p1642715335241"></a><a name="p1642715335241"></a>CheckLevel</p>
</td>
<td class="cellrowborder" valign="top" width="74.9%" headers="mcps1.2.3.1.2 "><p id="p14427173322419"><a name="p14427173322419"></a><a name="p14427173322419"></a>检查级别。取值为3或者5。</p>
<a name="ul13735192084113"></a><a name="ul13735192084113"></a><ul id="ul13735192084113"><li>CheckLevel＝3，只检查LiveID是否匹配。</li><li>CheckLevel＝5，检查LiveID是否匹配，Timestamp是否超时。</li></ul>
</td>
</tr>
<tr id="row193161838182916"><td class="cellrowborder" valign="top" width="25.1%" headers="mcps1.2.3.1.1 "><p id="p16316838142910"><a name="p16316838142910"></a><a name="p16316838142910"></a>IV</p>
</td>
<td class="cellrowborder" valign="top" width="74.9%" headers="mcps1.2.3.1.2 "><p id="p931718380296"><a name="p931718380296"></a><a name="p931718380296"></a>CBC对称加密算法依赖IV向量，随机生成的16位数字和字母组合，IV值长度为128位；CBC模式，PKCS7填充。</p>
</td>
</tr>
</tbody>
</table>

鉴权URL示例

```
rtmp://live.huaweitest1.com/live/8712345?auth_info=LpB4kdZfnOwfbpIgYVo4ABAU6CRUmV00OEARLlC7NLs%3D.79436d453636364e335941713330534e
```

其中，**LpB4kdZfnOwfbpIgYVo4ABAU6CRUmV00OEARLlC7NLs%3D**为加密串，**79436d453636364e335941713330534e**为EncodedIV。

## 代码示例<a name="section632515010576"></a>

以下以Java demo为例，生成鉴权URL中的“加密串.EncodedIV“。

```
import javax.crypto.Cipher;
import javax.crypto.spec.IvParameterSpec;
import javax.crypto.spec.SecretKeySpec;

import java.io.UnsupportedEncodingException;
import java.net.URLEncoder;

public class Main {

        public static void main(String[] args) {

		// data="$"+<Timestamp>+"$"+<LiveID>+"$"+<CheckLevel>，具体请参见“鉴权URL生成”
                String data = "$20190428110000$live/stream01$3";

                // 随机生成的16位数字和字母组合
		byte[] ivBytes = "yCmE666N3YAq30SN".getBytes();

                //在直播控制台配置的Key值
		byte[] key = "MyLiveKeyValue01".getBytes();

                String msg = aesCbcEncrypt(data, ivBytes, key);
		try {
			System.out.println(URLEncoder.encode(msg, "UTF-8") + "." + bytesToHexString(ivBytes));
		} catch (UnsupportedEncodingException e) {
			e.printStackTrace();
		}
	}

        private static String aesCbcEncrypt(String data, byte[] ivBytes, byte[] key) {
		try {
			SecretKeySpec sk = new SecretKeySpec(key, "AES");
			Cipher cipher = Cipher.getInstance("AES/CBC/PKCS5Padding");

                        if (ivBytes != null) {
				cipher.init(Cipher.ENCRYPT_MODE, sk, new IvParameterSpec(ivBytes));
			} else {
				cipher.init(Cipher.ENCRYPT_MODE, sk);
			}

                        return Base64.encode(cipher.doFinal(data.getBytes("UTF-8")));
		} catch (Exception e) {
			return null;
		}
	}

        public static String bytesToHexString(byte[] src) {
		StringBuilder stringBuilder = new StringBuilder("");
		if ((src == null) || (src.length <= 0)) {
			return null;
		}

                for (int i = 0; i < src.length; i++) {
			int v = src[i] & 0xFF;
			String hv = Integer.toHexString(v);
			if (hv.length() < 2) {
				stringBuilder.append(0);
			}
			stringBuilder.append(hv);
		}
		return stringBuilder.toString();
	}
}
```

以下是Base64类，用于将加密串进行编码。

```
public class Base64
{

    /** Base64编码表。*/
    private static char base64Code[] =
    {
        'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R',
        'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j',
        'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', '0', '1',
        '2', '3', '4', '5', '6', '7', '8', '9', '+', '/',};

    /**
     * 构造方法私有化，防止实例化。
     */
    private Base64()
    {
        super();
    }

    /**
     * Base64编码。将字节数组中字节3个一组编码成4个可见字符。
     * @param bytes 需要被编码的字节数据。
     * @return 编码后的Base64字符串。
     */
    public static String encode(byte[] bytes)
    {
        int a = 0;

        // 按实际编码后长度开辟内存，加快速度
        StringBuffer buffer = new StringBuffer(((bytes.length - 1) / 3) << 2 + 4);

        // 进行编码
        for (int i = 0; i < bytes.length; i++)
        {
            a |= (bytes[i] << (16 - i % 3 * 8)) & (0xff << (16 - i % 3 * 8));
            if (i % 3 == 2 || i == bytes.length - 1)
            {
                buffer.append(Base64.base64Code[(a & 0xfc0000) >>> 18]);
                buffer.append(Base64.base64Code[(a & 0x3f000) >>> 12]);
                buffer.append(Base64.base64Code[(a & 0xfc0) >>> 6]);
                buffer.append(Base64.base64Code[a & 0x3f]);
                a = 0;
            }
        }

        // 对于长度非3的整数倍的字节数组，编码前先补0，编码后结尾处编码用=代替，
        // =的个数和短缺的长度一致，以此来标识出数据实际长度
        if (bytes.length % 3 > 0)
        {
            buffer.setCharAt(buffer.length() - 1, '=');
        }
        if (bytes.length % 3 == 1)
        {
            buffer.setCharAt(buffer.length() - 2, '=');
        }
        return buffer.toString();
    }

}
```

