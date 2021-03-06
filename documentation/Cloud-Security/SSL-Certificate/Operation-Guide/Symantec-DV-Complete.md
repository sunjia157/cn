# 信息补全

1、进入控制台，从左侧导航栏依次选择 **云安全** -> **SSL数字证书** -> **申购管理**进入SSL数字证书申购管理页面

![申购管理](/image/SSL-Certification/申购管理.png)

2、购买完成后，证书应处于 **待补全信息** 的状态，点击 **补全信息**，弹出以下页面

![补全信息](/image/SSL-Certification/Symantec-DV-补全信息.png)

3、按照提示填写证书名称、绑定域名、校验方式等信息。其中，申请者需要对绑定的域名具有所有权，校验方式可以选择 **DNS校验**或者 **文件校验**的方式，两种校验方式简介以及操作步骤如下。

## DNS校验

需要您手动为域名添加一条TXT类型的解析记录，来验证域名所有权。

操作步骤：

- 从DNS解析服务商网站进入DNS域名解析页面

- 添加云解析，添加解析内容，包括网址信息，将记录类型选择为TXT，在记录值中输入验证时获取的一串记录值
  
  ![添加解析内容](/image/SSL-Certification/添加解析内容.png)

- 等待解析生效即可


## 文件校验

需要您手动在该域名站点的指定目录上传指定的文件，来验证域名所有权。

操作步骤：

- 复制文件内容：点击 **复制** 按钮,内容有效期一般为24小时。

![文件内容](/image/SSL-Certification/文件内容.png)

- 创建目录
  - 登录服务器，创建指定的文件目录（your-domain.com/.well-known/pki-validation/fileauth.txt）
  - 将文件内容拷贝到指定的文件目录中
  
- 配置检测
  - HTTP配置检测链接：http://您的域名/.well-known/pki-validation/fileauth.txt 

请确保您的主机服务商没有屏蔽国外访问。如已屏蔽，请联系主机服务商。

配置好之后，请用浏览器访问地址是否正常输出内容。

**常见的错误**：
- 文件内容不正确；
- 内容看起来正确，但并不正确，原因是里面包含了HTML元素；
- 原始地址发生了跳转；
- 内容已经过期。
