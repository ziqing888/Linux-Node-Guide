# 1- VPS 购买指南

参与节点测试网的第一步就是需要一个 VPS 服务器。

为了购买 VPS（云服务器），我推荐一些国外和伊朗的提供商，支持加密货币支付或传统支付方式。

| 排名 | 提供商 | 支付方式 | 描述 |
| :--- | :--- | :--- | :--- |
| 1 | Hetzner | `信用卡 - 需要KYC验证` | `最佳托管服务，但价格较高`，[拍卖服务器](https://www.hetzner.com/sb/)（最低 $30）性能好 |
| 2 | Contabo | `信用卡 - 需要KYC验证` | `价格便宜，但部分节点存在带宽问题` |
| 3 | [Hostbrr](https://my.hostbrr.com/order/forms/a/NTMxNw==) | `加密货币` | `价格适中，性能好` |
| 4 | [PQhosting](https://pq.hosting/?from=800121) | `加密货币` | `性能好，部分服务器价格便宜` |
| 5 | [Aeza](https://aeza.net/?ref=392339) | `加密货币` | `按小时计费的服务器最佳，有时能找到优质服务器` |
| 6 | [Bartarvs](https://bartarvs.net/) | `伊朗里亚尔 - 加密货币` | `伊朗 - Myloc 和 Contabo 云服务器价格便宜，但 Myloc 性能低` |

> *免责声明：此列表仅基于个人经验，非推荐。*

---

# 2- 系统配置推荐

购买 VPS 前，需考虑一些组件以选择所需系统：

* `CPU`：通常 4 核至 16 核
* `内存`：通常 4GB 至 32GB
* `硬盘`：节点通常要求硬盘空间较大，最低建议为 60GB，建议 SSD
* `操作系统`：最好为 `Ubuntu`，通常 `Ubuntu 22` 适用于大多数项目
* VPS 必须是 IPv4 且不能是 NAT

---

# 3- 购买 VPS 的示例

为了更好地理解流程，我们将从两个提供商购买 VPS 服务器。**这不是推荐，只是演示过程。**

## Hostbrr

列出 Hostbrr 的一些服务器选择：

- 高内存：[内存优化 VPS](https://my.hostbrr.com/order/main/packages/largeram/?group_id=23)
- 更佳带宽和内存：[RAM 优化 - 高级](https://my.hostbrr.com/order/main/packages/largeram/?group_id=38)
- 性能好的 CPU：[AMD Ryzen 9 7950XD](https://my.hostbrr.com/order/main/packages/vps7950/?group_id=14)
- 更便宜的 CPU：[AMD Ryzen 9 5950X](https://my.hostbrr.com/order/main/packages/vpsgermany/?group_id=13)

### 步骤：
1. 选择 AMD Ryzen 9 5950X（$14.99/月）4 vCore，8GB RAM，150GB 存储。
2. 注册信息，通过 Metamask 使用 Coinbase 支付。
3. 激活后，手动安装 Ubuntu 22。
4. IP 和密码会通过邮件发送。

---

## Bartarvs

- 列出 Bartarvs 的云服务器：[云服务器列表](https://bartarvs.net/server/cloud-server/)
- 低成本普通性能：[MyLoc](https://bartarvs.net/cloud-server-myloc-linux/)
- 便宜且性能好：[Contabo](https://bartarvs.net/cloud-server-contabo/)

在购买之前配置：选择 Ubuntu 22 和更大存储 SSD。

---

# 4- 如何连接到 VPS

通过 SSH 连接到 VPS 需要客户端，如 Mobaxterm、Termius 或 Putty。

1. **获取连接信息**：
   - **IP 地址**：激活后邮件提供
   - **端口**：默认 SSH 端口为 22
   - **用户名**：通常为 `root`
   - **密码**：激活后邮件提供

2. **使用 Mobaxterm 连接**：
   - 打开 Mobaxterm，点击 `Session`，选择 `SSH`
   - 输入服务器 IP（如 `root@IP`），端口为 `22`
   - 点击 `OK` 后，输入密码（使用鼠标中键粘贴）

3. **使用 Mobaxterm 的 SFTP**：
   - Mobaxterm 左侧可以查看 `/root/` 目录及文件。

