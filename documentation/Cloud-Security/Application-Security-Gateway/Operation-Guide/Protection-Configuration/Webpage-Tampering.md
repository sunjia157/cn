# 网页防篡改

**功能描述**

​    网页防篡改采用强制静态缓存锁定和更新机制，对网站特定页面进行保护，即使源站相关网页被篡改，依然能够返回给用户缓存页面。当前该功能属于公测阶段，在基础版中免费提供。

**操作步骤**

​     1、进入控制台实例管理页面，点击防护配置接入防护选项卡配置页面，点击网页防篡改设置。

![image.png](https://img1.jcloudcs.com/cms/ab29442e-f406-442d-9334-4db0db4a1b4b20180817111409.png)

​    **字段说明**：

​    **URL**:防篡改页面的URL。

​    **防篡改次数**：添加防篡改页面后，防篡改生效的次数

​    **防护状态**：该规则是否生效

​    **操作说明**：   

​            更新缓存，点击对防护页面的内容进行进行更新，防护页面将在第一次访问源站时缓存相关的页面信息。

​            编辑：对规则进行修改。

​            删除：删除对应规则。

​    2、点击添加规则，填写规则名称和需要进行防篡改的URL

​    ![image.png](https://img1.jcloudcs.com/cms/1270e388-4827-4e1c-9244-0500785b4f1f20180817111645.png)