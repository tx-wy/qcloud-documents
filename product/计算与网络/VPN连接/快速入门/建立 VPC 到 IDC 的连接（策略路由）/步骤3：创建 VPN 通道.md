本文为您介绍如何创建 VPN 通道，您可通过如下视频了解 VPN 通道的相关操作。
<div class="doc-video-mod"><iframe src="https://cloud.tencent.com/edu/learning/quick-play/1786-20144?source=gw.doc.media&withPoster=1&notip=1"></iframe></div>


## 操作步骤
1. 登录 [私有网络控制台](https://console.cloud.tencent.com/vpc/vpc?rid=1)。
2. 在左侧目录中单击 **VPN 连接** > **VPN 通道**，进入管理页。
3. 选择对应的地域和私有网络，如示例中的**广州**和 `TomVPC`，单击**+新建**。
 ![](https://main.qcloudimg.com/raw/736f88fd2bbf5e75033d77fcf372586f.png)
4. 输入通道名称（如：TomVPNConn），选择 VPN 网关`TomVPNGw`与对端网关`TomVPNUserGw`，并输入预共享密钥（如：`123456`），单击**下一步**。
>?标签为选配，请保持默认。
>
![](https://qcloudimg.tencent-cloud.cn/raw/0a0f25810d4d5a0c26529cc0f320775f.png)
5. 选择通信模式，并输入 SPD 策略来限制本端哪些网段和对端哪些网段通信，在本例中本端网段即为子网 A 的网段`192.168.1.0/24`，对端网段为`10.0.1.0/24`，单击**下一步**。
![](https://qcloudimg.tencent-cloud.cn/raw/0a9b332c3936725cc0a1bbf9e238f311.png)
6. 配置 IKE 参数，需要与本地 IDC 侧配置一致，参数具体信息请参见 [创建 VPN 通道](https://cloud.tencent.com/document/product/554/52864)。本示例中默认的 IKE 参数已与 IDC 侧相匹配。如果不需要高级配置，可直接单击**下一步**。
 ![](https://main.qcloudimg.com/raw/c370884071d8dd5424be80bbef1e9aec.png)
7. 配置 IPSec 参数，需要与本地 IDC 侧配置一致，参数具体信息请参见 [创建 VPN 通道](https://cloud.tencent.com/document/product/554/52864)。本示例中默认的 IPSec 参数已与 IDC 侧相匹配。如果不需要配置，可直接单击**完成**。
 ![](https://main.qcloudimg.com/raw/6c67f435c015fb6d2e03ed96dc61b7f7.png)
8. 创建成功后，返回 VPN 通道列表页，单击**更多**，选择**下载配置文件**并完成下载。
![](https://qcloudimg.tencent-cloud.cn/raw/96a92a39e1f65c42eadd069882e57131.png)
