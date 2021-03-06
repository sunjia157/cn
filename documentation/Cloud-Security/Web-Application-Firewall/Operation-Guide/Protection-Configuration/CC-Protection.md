# CC安全防护

CC防护简介

CC安全防护帮助您防护针对页面请求的CC攻击，应用独家算法防护引擎，结合大数据，秒级拦截机器人，恶意CC攻击。

### **功能描述**

CC安全防护可以拦截机器恶意CC攻击，并提供不同模式的防护策略：正常、攻击紧急。

将网站接入WAF后，您可以为其开启CC安全防护，并根据实际需求调整相应防护策略。

### **操作步骤**

参照以下步骤，配置CC安全防护模式：

**说明：** 执行以下操作前，请确保已将网站接入WAF进行防护。具体操作请参考CNAME接入指南。

1. 登录[京东云Web应用防火墙控制台](https://cloudwaf-console.jdcloud.com)。

2. 前往**网站配置**页面。

3. 选择要操作的域名，单击其操作列下的**防护配置**。

4. 在**CC安全防护**下，开启防护，并选择相应防护模式： 
         **说明：** 如果您需要关闭防护功能，可在此处关闭防护。![img](https://github.com/jdcloudcom/cn/blob/edit/image/waf-img/cc-web1.png)

5. - **正常**：默认使用正常模式。针对特别异常的请求进行拦截。建议您在网站无明显流量异常时采用此模式。
   - **攻击紧急**：当出现网站响应缓慢，流量、CPU、内存等指标异常时，可以选择攻击紧急模式。


 
