# 更新訂閱鏈接失效解決方法：

Nginx請關閉WAF防火墻，如果有cloudflare請設置以下頁面規則
```
您的網域.com/ssr-download/ssr/*     （此為下載程式鏈接）
您的網域.com/link/*                 （此為頂級域名訂閱鏈接，具體請按照您網域）
www.您的網域.com/link/*             （此為二級域名訂閱鏈接，具體請按照您網域）
```


# TG機器人重複解碼解決方法：
請保持禁用以下PHP函數：
```
passthru
exec
system
chroot
chgrp
chown
shell_exec
popen
ini_alter
ini_restore
dl
openlog
syslog
readlink
symlink
popepassthru
```