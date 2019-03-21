---

copyright:
  years: 2017, 2019
lastupdated: "2019-03-21"

---


# 在 Windows 中使用 iSCSI 软件启动器连接到 DTS 设备
{: #mountingDTSWindows}

要在 Windows 中与 iSCSI LUN 进行交互，用户必须使用 iSCSI 软件启动器（Microsoft 的专有 iSCSI 工具）来连接到存储器。对于 Windows Server 2008、Windows Vista 或更新版本的用户，iSCSI 软件启动器已内置于操作系统中。Windows Server 2003、Windows XP 和 Windows 2000 的用户必须先下载该启动器，然后再启动此过程。

## 连接到 iSCSI LUN

1. 从 {{site.data.keyword.slportal}}，检索想要连接的存储设备的 **iSCSI 用户名、密码和存储地址**。
2. 启动 iSCSI 启动器。
3. 单击**发现**。
4. 在**目标门户网站**部分中，单击**添加**。
5. 在 **IP 地址或 DNS 名称**字段中，输入 **iSCSI IP 地址**。
6. 单击**高级**。
7. 更新 iSCSI 登录信息。
   - 选中 **CHAP 登录信息**复选框以启用 CHAP 登录。
   - 在**用户名**字段中输入 iSCSI 用户名。
   - 在**目标私钥**字段中输入 iSCSI 密码。
   - 单击**确定**两次。
8. 单击**目标**
9. 从**目标**列表中选择新添加的 iSCSI。
10. 单击**登录**。这将显示**登录到目标**窗口。
11. 选中**系统引导时自动还原此连接**，以设置在重新启动之间持久保持连接。
12. 单击**高级**。
13. 更新 iSCSI 登录信息。
    - 选中 **CHAP 登录信息**复选框以启用 CHAP 登录。
    - 在**用户名**字段中输入 iSCSI 用户名。
    - 在**目标私钥**字段中输入 iSCSI 密码。
    - 单击**确定**两次。
14. 验证“目标”选项卡上新的 iSCSI 目标是否显示为“已连接”。
    - 如果 iSCSI 目标显示为**已连接**，那么单击**确定**。现在，您的 iSCSI LUN 已连接
    - 如果 iSCSI 目标未显示为**已连接**，请重复所有先前步骤以重置连接。
