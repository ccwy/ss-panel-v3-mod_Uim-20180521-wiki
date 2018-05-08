# 概述

~~明明Telegram都给了官方登陆方式了，为什么还要用那么麻烦的扫码和数字呢？~~  
方便快捷，一次授权，后续直接跳转，：）
![登陆效果](http://ww1.sinaimg.cn/large/d0953529ly1fr3yx5wg36j20n00hdq5r.jpg)

# 准备工作

![机器人操作截图](http://ww1.sinaimg.cn/large/d0953529gy1fr3z32hg9fj20hm0cnq6t.jpg)

超简单的有木有！
- 给 [@Botfather](https://t.me/botfather) 发一句 `/setdomain`
- 选你要设置的机器人
- 回复你的网站**域名**
    - 比如，你的登陆页面是`https://example.com/auth/login`,你只要发给他`example.com`就好了
    - 如果是`https://xxx.example.com/auth`，那么是`xxx.example.com`
- 起飞！

# 样式调整

什么？你怎么这么多事情……  
指南在[这里](https://core.telegram.org/widgets/login)，什么显示头像，名字，字体大小什么的  
然后到 `login.tpl` 结尾自己改吧  

# 最后的补充

- 这玩意用的是`async`载入的，不会阻塞页面其他内容加载
- 别试图自己反代这个脚本或者什么重新适配，后面的故事远不止如此，不能科学上网的话基本是用不了滴，别想了

