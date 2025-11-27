+++
date = '2025-11-27T21:30:19+08:00'
draft = false
title = 'Cloudfare Hugo'
+++

# 从0到1在CloudFare上部署Hugo站点

前置条件：

1. 你已经拥有一个hugo项目，并且托管在github（或gitlab，本文以github为例）
2. 注册一个CloudFare账号

# 1️⃣CloudFare部署Hugo

[点击跳转CloudFare登录地址](https://dash.cloudflare.com/login)

1. 点击【Add】，选择【Pages】，新建一个Pages
![](/cloudfare/step1.png)
2. 选择从github【get started】
![](/cloudfare/step2.png)
3. 如果你没有认证过，这里首先会让你登录github进行授权。授权完毕后就是如下页面。你可以选择到自己的仓库。按照下图步骤操作
![](/cloudfare/step3.png)
![](/cloudfare/step4.png)


4. 执行如下命令查询`hugo`的版本
    ```shell
    # 查看hugo版本的命令，+后不是版本，只有小数点和数字表示版本
    # 如我这里输出hugo v0.147.4+extended+withdeploy darwin/arm64 BuildDate=2025-05-20T10:41:19Z VendorInfo=brew
    # 那我得版本就是0.147.4
    hugo version
    ```
    ![](/cloudfare/step5.png)

5. 点击【save and deploy】按钮进入下一步<br/>等待几个步骤加载后，出现如下success字样表示网站部署成功。

    ![](/cloudfare/step6.png)

# 2️⃣配置域名

![](/cloudfare/step7.png)

未完待续……




