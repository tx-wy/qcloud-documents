## 操作场景
ASP.NET 应用镜像提供了开源的服务端 Web 应用程序框架，可用于构建动态网页、应用和服务。您可使用该应用镜像创建实例，搭建跨境电商环境。

<dx-alert infotype="explain" title="">
- 本文示例 ASP.NET 应用镜像底层基于 Windows Server 2019操作系统。应用镜像会进行不定期更新，请以购买页面实际镜像信息为准。
- 该镜像最少需要50GB SSD系统盘，请注意选择实例套餐。
</dx-alert>



## 操作步骤
1. 登录 [轻量应用服务器控制台](https://console.cloud.tencent.com/lighthouse)。配置如下参数：
 - **地域、可用区**：建议选择靠近目标客户的地域及可用区，降低网络延迟、提高您的客户的访问速度。例如目标客户在 “深圳”，地域选择 “广州”。
 - **镜像**：选择 “ASP.NET” 应用镜像。
 - **实例套餐**：按照所需的服务器配置（CPU、内存、系统盘、峰值带宽、每月流量），选择一种实例套餐。
 - **实例名称**：自定义实例名称，若不填则默认使用所选镜像名称。批量创建实例时，连续命名后缀数字自动升序。例如，填入名称为 LH，数量选择3，则创建的3个实例名称为 LH1、LH2、LH3。
 - **购买时长**：默认1个月。
 - **购买数量**：默认1台。
2. 单击**立即购买**，并根据页面提示提交订单完成支付。

## 相关操作

### 查看实例各项应用配置信息
1. 登录 [轻量应用服务器控制台](https://console.cloud.tencent.com/lighthouse)。
2. 在服务器列表中，选择并进入使用 ASP.NET 应用镜像创建的实例详情页。
3. 选择**应用管理**页签，进入应用管理详情页。如下图所示：
![](https://qcloudimg.tencent-cloud.cn/raw/9533f63d2c3010eb4e080182315448d8.png)
您可以在此页面查看应用内软件的各项配置信息。例如：
 - ASP.NET、MySQL、Visual Studio 等软件的安装地址。
 - MySQL 管理员账号及登录密码获取方式。

### 使用 FTP 工具上传代码并调试
ASP.NET 应用镜像中已包含 FileZilla 应用软件，您可通过该软件连接本地机器，上传自己的网站代码，并进行测试调试。

### 域名与 DNS 解析设置
您可以给自己的网站设定一个单独的域名。用户可以使用易记的域名访问您的网站，而不需要使用复杂的 IP 地址。有些用户搭建网站仅用于学习，那么可使用 IP 直接访问网站，但不推荐这样操作。

如果您已有域名或者想要通过域名来访问您的网站，请参考以下步骤：
1. 通过腾讯云 [购买域名](https://dnspod.cloud.tencent.com/?from=qcloud)，具体操作请参考 [域名注册](https://cloud.tencent.com/document/product/242/9595)。
2. 进行 [网站备案](https://cloud.tencent.com/product/ba?from=qcloudHpHeaderBa&fromSource=qcloudHpHeaderBa)。 
域名指向中国境内服务器的网站，必须进行网站备案。在域名获得备案号之前，网站是无法开通使用的。您可以通过腾讯云免费进行备案，审核时长请参考 [备案审核](https://cloud.tencent.com/document/product/243/19650)。
3. 通过腾讯云 [DNS解析 DNSPod](https://cloud.tencent.com/product/cns?from=qcloudHpHeaderCns&fromSource=qcloudHpHeaderCns) 配置域名解析。具体操作请参考 [A 记录](https://cloud.tencent.com/document/product/302/3449)，将域名指向一个 IP 地址（外网地址）。

### 开启 HTTPS 访问
可参考 [如何选择 SSL 证书安装部署类型](https://cloud.tencent.com/document/product/400/4143) 文档，为您的网站安装 SSL 证书并开启 HTTPS 访问。

