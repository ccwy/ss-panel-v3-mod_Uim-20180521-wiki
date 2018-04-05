原文 https://91vps.bid/2017/06/09/alipay_f2f_ss_panel_mod/
如需代签约当面付请Telegram联系[守夜人](https://t.me/shouyeren)

### 支付宝付款接口配置

```
$System_Config['f2fpay_app_id']='2017221985';
$System_Config['f2fpay_p_id']='20887023';
$System_Config['alipay_public_key']='MIIBxxxxxxxxxxxxxx';
$System_Config['merchant_private_key']='MIIExxxxxxxxxxxxxxxxxxx';
```

一共有五个位置要填写：

#### 密钥生成工具请使用支付宝官方工具，注意红框内的选项。

![img](http://cdn.mmmxcc.cn/blog/20170610/211328759.png?imageView2/0/format/webp/interlace/1/q/75|watermark/2/text/ZmVpeWFuZy5saQ==/font/Y29taWMgc2FucyBtcw==/fontsize/500/fill/IzAzQTlGNA==/dissolve/35/gravity/SouthEast/dx/10/dy/10|imageslim)

#### 第一个位置： `$System_Config['f2fpay_app_id']=''`

这个是支付宝开放平台里的APPID，开通收款码服务后进入支付宝开放平台，签约**自研开发者**后进入开发者中心新建一个app提交审核后记下APPID

#### 第二个位置： `$System_Config['f2fpay_p_id']`

这个是收款的支付宝账号，用来确认阿里消息正确性的。
https://openhome.alipay.com/platform/keyManage.htm?keyType=partner
签约管理里合作伙伴身份PID

#### 第三个位置： `$System_Config['alipay_public_key']`

指的是这里的**支付宝公钥**，注意是**支付宝公钥**。
![img](http://cdn.mmmxcc.cn/blog/20170610/211039761.png?imageView2/0/format/webp/interlace/1/q/75|watermark/2/text/ZmVpeWFuZy5saQ==/font/Y29taWMgc2FucyBtcw==/fontsize/500/fill/IzAzQTlGNA==/dissolve/35/gravity/SouthEast/dx/10/dy/10|imageslim)

#### 第四个位置： `$System_Config['merchant_private_key']`

这个是你**自己的私钥**。