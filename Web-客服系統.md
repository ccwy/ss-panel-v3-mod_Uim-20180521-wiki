# crisp

註冊地址：https://crisp.chat/

~~路徑1：/resources/views/material/header.tpl（最後行代碼）~~

~~路徑2：/resources/views/material/user/main.tpl （最後行代碼）~~

~~```
 <script type="text/javascript"> window.$crisp=[];window.CRISP_WEBSITE_ID="您的ID";(function(){ d=document;s=d.createElement("script"); s.src="https://client.crisp.chat/l.js"; s.async=1;d.getElementsByTagName("head")[0].appendChild(s);})(); </script>
```~~

~~請把“您的ID”更換為您的ID~~

### 以上已废止

现直接在`config/.config.php`中的客服系统下填入相关信息即可

其中

`$System_Config['enable_crisp']='false'`为是否开启 ，`true`为开启，`false`为关闭

`$System_Config['crisp_id']='null'`为ID设置，中将`null`替换为自己的ID即可

ID查看路徑：crisp.chat-->設置-->設置網站-->顯示整合性-->HTML