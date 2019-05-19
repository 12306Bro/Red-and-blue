## 概要

------

安全标识符 (SID) 是用于标识安全主体或 Windows 操作系统中的安全组的可变长度的唯一值。已知的 Sid 是识别普通用户的 Sid 的一组或通用组。在所有操作系统，其值将保持不变。

此信息可用于涉及安全的问题进行故障排除。也是用于 ACL 编辑器中可能出现的潜在的显示问题。SID 可能会显示在 ACL 编辑器，而不是以用户或组的名称。

## 详细信息

------

以下是众所周知的 Sid:

- SID: S-1-0
  名称： 空机构
  说明： 标识符颁发机构。

- SID: S-1-0-0
  名称： 没有人
  说明： 没有安全主体。

- SID: S-1-1
  名称： 世界机构
  说明： 标识符颁发机构。

- SID: S-1-1-0
  名称： 所有人
  说明： 包括所有甚至匿名用户和来宾用户组。成员资格是由操作系统控制的。

  注意：默认情况下，Everyone 组不再包含计算机正在运行 Windows XP Service Pack 2 (SP2) 上的匿名用户。

- SID: S-1-2
  名称： 本地机构
  说明： 标识符颁发机构。

- SID: S-1-2-0

  名称： 本地

  说明： 包括所有本地登录的用户组。

- SID: S-1-2-1

  名称： 控制台登录

  说明： 包括到物理控制台登录用户的组。

  注意：7 和 Windows Server 2008 R2 在窗口中添加

- SID: S-1-3
  名称： 创建者颁发机构
  说明： 标识符颁发机构。

- SID: S-1-3-0
  名称： 创建者所有者
  说明： 父系的可继承的访问控制项 (ACE) 中的占位符。ACE 继承时，系统将此 SID 替换对象的创建者的 SID。

- SID: S-1-3-1
  名称： 创建者组
  说明： 父系的可继承 ACE 中的占位符。当继承 ACE 时，系统将此 SID 替换 SID 为主要对象的创建者的组。仅 POSIX 子系统所用的主要组。

- SID: S-1-3-2
  名称： 创建者所有者服务器
  说明： 此 SID 不在 Windows 2000 中使用。

- SID: S-1-3-3
  创建者组服务器名称：
  说明： 此 SID 不在 Windows 2000 中使用。

- SID: S-1-3-4 名： 所有者权限

  说明： 一组，表示该对象的当前所有者。当执行此 SID 的 ACE 应用于对象时，系统将忽略隐式 READ_CONTROL 和 WRITE_DAC 为对象的所有者的权限。

- SID: S-1-5-80-0
  所有服务的名称：
  说明： 一组包含在系统上配置的所有服务进程。成员资格是由操作系统控制的。

  注意：Windows Vista 和 Windows Server 2008 中添加

- SID: S-1-4
  名称： 非唯一授权机构
  说明： 标识符颁发机构。

- SID: S-1-5
  名称： NT 机构
  说明： 标识符颁发机构。

- SID: S-1-5-1
  名称： 拨号
  说明： 包括通过拨号连接登录的所有用户组。成员资格是由操作系统控制的。

- SID: S-1-5-2
  名称： 网络
  说明： 包括通过网络连接登录的所有用户组。成员资格是由操作系统控制的。

- SID: S-1-5-3
  名称： 批处理
  说明： 包括所有通过批队列工具登录的用户组。成员资格是由操作系统控制的。

- SID: S-1-5-4
  名称： 交互式
  说明： 包括所有以交互方式登录的用户组。成员资格是由操作系统控制的。

- SID: S-1-5-5-X-Y
  名称： 登录会话
  说明： 登录会话。为每个会话中，这些 Sid 的 X 和 Y 值是不同的。

- SID: S-1-5-6
  名称： 服务
  说明： 包括所有安全主体作为服务登录的组。成员资格是由操作系统控制的。

- SID: S-1-5-7
  名称： 匿名
  说明： 包括匿名登录的所有用户组。成员资格是由操作系统控制的。

- SID: S-1-5-8
  名称： 代理服务器
  说明： 此 SID 不在 Windows 2000 中使用。

- SID: S-1-5-9
  名称： 企业域控制器
  说明： 包括使用 Active Directory 目录服务林中的所有域控制器组。成员资格是由操作系统控制的。

- SID: S-1-5-10
  名称： 主体自身
  描述： 在一个帐户对象或组在 Active Directory 中的对象可继承的 ACE 中的占位符。ACE 继承时，系统将此 SID 替换持有帐户安全主体的 SID。

- SID: S-1-5-11
  已验证的用户的名称：
  说明： 包括登录时其身份已通过身份验证的所有用户组。成员资格是由操作系统控制的。

- SID: S-1-5-12
  名称： 受限制的代码
  说明： 此 SID 是保留供将来使用。

- SID: S-1-5-13
  终端服务器用户名称：
  说明： 包括所有登录到终端服务服务器的用户组。成员资格是由操作系统控制的。

- SID: S-1-5-14
  名称： 远程交互式登录
  说明： 包括通过终端服务登录登录的所有用户组。

- SID: S-1-5-15
  此组织名称：
  说明： 包括所有来自同一组织的用户组。仅包括与广告客户，只添加的 Windows Server 2003 或更高版本的域控制器。

- SID: S-1-5-17
  此组织名称：
  说明： 默认 Internet Information Services (IIS) 用户使用的帐户。

- SID: S-1-5-18
  名称： 本地系统
  说明： 服务帐户使用的操作系统。

- SID: S-1-5-19
  名称： NT 机构
  说明： 本地服务

- SID: S-1-5-20
  名称： NT 机构
  描述： 网络服务

- SID: S 1 5 21-**域**-500
  名称： 管理员
  描述： 系统管理员用户帐户。默认情况下，它是唯一的用户帐户能够完全控制该系统。

- SID: S 1 5 21-**域**-501
  名称： 来宾
  说明： 用户帐户的人不具有单独的帐户。此用户帐户不需要密码。默认情况下，Guest 帐户被禁用。

- SID: S 1 5 21-**域**-502
  名称： KRBTGT
  说明： 使用密钥分发中心 (KDC) 服务的服务帐户。

- SID: S 1 5 21-**域**-512
  名称： 域管理员
  说明： 其成员被授权管理域全局组。默认情况下，域管理员组是所有已加入到域中，域控制器的计算机上管理员组的成员。域管理员已创建的组的任何成员的任何对象的默认所有者。

- SID: S 1 5 21-**域**-513
  名称： 域用户
  说明： 全局组，默认情况下，包括域中所有用户帐户。在域中创建用户帐户时，它是默认添加到此组。

- SID: S 1 5 21-**域**-514
  名称： 域来宾
  说明： 一个全局组，默认情况下，都有只有一个成员，则域的内置来宾帐户。

- SID: S 1 5 21-**域**-515
  名称： 域计算机
  说明： 全局组，其中包括所有客户端和加入域的服务器。

- SID: S 1 5 21-**域**-516
  域控制器名称：
  说明： 一个全局组包括域中所有域控制器。默认情况下，新的域控制器都添加到此组。

- SID: S 1 5 21-**域**-517
  名称： 证书发行者
  说明： 全局组，其中包括所有的计算机正在运行企业证书颁发机构。证书发布者有权在 Active Directory 中发布证书的用户对象。

- SID: S 1 5 21-**根域**-518
  名称： 架构管理员
  说明： 在本机模式域; 通用组在混合模式域的全局组。该组有权在 Active Directory 中进行架构更改。默认情况下，该组的唯一成员是林根域的管理员帐户。

- SID: S 1 5 21-**根域**-519
  名称： 企业管理员
  说明： 在本机模式域; 通用组在混合模式域的全局组。该组有权在 Active Directory 中进行全林性更改，例如添加子域。默认情况下，该组的唯一成员是林根域的管理员帐户。

- SID: S 1 5 21-**域**-520
  名称： 组策略创建者所有者
  说明： 全局组被授权可在活动目录中创建新的组策略对象。默认情况下，该组的唯一成员是管理员。

- SID: S 1 5 21-**域**-526
  名称： 密钥管理员
  说明：安全组。此组的目的是要委派的 msdsKeyCredentialLink 属性上的写访问权限。组适用于在方案中使用的受信任的外部机构 （如 Active Directory 联合服务） 负责修改此属性。只有受信任的管理员应成为此组的成员。

- SID: S 1 5 21-**域**-第 527
  名称： 企业密钥管理
  说明：安全组。此组的目的是要委派的 msdsKeyCredentialLink 属性上的写访问权限。组适用于在方案中使用的受信任的外部机构 （如 Active Directory 联合服务） 负责修改此属性。只有受信任的管理员应成为此组的成员。

- SID: S 1 5 21-**域**-553
  名称： RAS 和 IAS 服务器
  说明： 本地域组。默认情况下，此组没有任何成员。此组中的服务器具有读取帐户限制和用户对象的读取登录信息访问 Active Directory 域本地组中。

- SID: S-1-5-32-544
  名称： 管理员
  说明： 内置组。在操作系统的初始安装后, 组的唯一成员是管理员帐户。当计算机加入域时，域管理员组被添加到管理员组中。域控制器服务器时，企业管理员组也被添加到管理员组中。

- SID： S-1-5-32-545
  名称： 用户
  说明： 内置组。在操作系统的初始安装之后, 的唯一成员是经过身份验证的用户组。当计算机加入域时，域用户组添加到计算机上的用户组。

- SID: S-1-5-32-546
  名称： 客人
  说明： 内置组。默认情况下，唯一的成员是 Guest 帐户。来宾组允许偶尔或一次性用有限特权的计算机的内置来宾帐户登录的用户。

- SID: S-1-5-32-547
  名称： 超级用户
  说明： 内置组。默认情况下，组没有任何成员。超级用户可以创建本地用户和组;修改和删除他们所创建的; 的帐户和超级用户、 用户和来宾组中删除用户。高级用户还可以安装程序;创建、 管理和删除本地打印机;创建和删除文件共享。

- SID: S-1-5-32-548
  名称： 帐户操作员
  描述： 一个内置组仅在域控制器存在。默认情况下，组没有任何成员。默认情况下，帐户操作员具有创建、 修改和删除用户、 组和所有容器和 Active Directory 单位除内置容器和域控制器 OU 中的计算机帐户的权限。帐户操作员没有权限修改管理员和域管理员组中，他们也没有修改这些组的成员帐户的权限。

- SID: S-1-5-32-549
  名称： 服务器操作员
  描述： 一个内置组仅在域控制器存在。默认情况下，组没有任何成员。服务器操作员可以登录到服务器上以交互方式;创建和删除网络共享;启动和停止服务;备份和还原文件。格式化硬盘的计算机;然后关闭计算机。

- SID: S-1-5-32-550
  名称： 打印操作员
  描述： 一个内置组仅在域控制器存在。默认情况下，唯一的成员是域用户组。打印操作员可以管理打印机和文档队列。

- SID: S-1-5-32-551
  名称： 备份操作员
  说明： 内置组。默认情况下，组没有任何成员。备份操作员可以备份和还原的计算机，无论使用什么权限保护这些文件的所有文件。备份操作员还可以登录到计算机上并将其关闭。

- SID: S-1-5-32-552
  名称： 复制器
  说明： 内置的组，它由文件复制服务在域控制器上。默认情况下，组没有任何成员。无法将用户添加到该组中。

- SID: S-1-5-64-10
  名称： NTLM 身份验证
  描述： 一个 SID 的 NTLM 身份验证软件包经过身份验证的客户端时使用

- SID: S-1-5-64-14
  名称： SChannel 身份验证
  描述： 频道身份验证软件包经过身份验证的客户端时使用 SID。

- SID: S-1-5-64-21
  名称： 摘要式身份验证
  说明： 在摘要式身份验证软件包经过身份验证的客户端时使用 SID。

- SID: S-1-5-80
  NT 服务名称：
  描述： 一个 NT 服务帐户前缀

- SID: S-1-5-80-0
  SID S-1-5-80-0 = SERVICES\ALL NT 服务
  所有服务的名称：
  说明： 一组包含在系统配置的所有服务进程。成员资格是由操作系统控制的。

  注意：添加到 Windows Server 2008 R2 中

- SID: S-1-5-83-0
  名称： NT 虚拟 MACHINE\Virtual 机
  说明： 内置组。安装 Hyper-V 角色时，将创建组。在组中的成员资格被维护 Hyper-V 管理服务 (VMM)。此组所需的"创建符号链接"权限 (SeCreateSymbolicLinkPrivilege)，并还"作为服务登录"右 (SeServiceLogonRight)。

  注意：Windows 8 和 Windows Server 2012 中添加

- SID: S-1-16-0
  名称： 不受信任的强制性级别
  描述： 一个不受信任的完整性级别。Windows Vista 和 Windows Server 2008 中添加注释

  注意：Windows Vista 和 Windows Server 2008 中添加

- SID: S-1-16-4096
  名称： 低强制性级别
  说明： 低完整性级别。

  注意：Windows Vista 和 Windows Server 2008 中添加

- SID: S-1-16-8192
  名称： 中等强制性级别
  说明： 中等完整性级别。

  注意：Windows Vista 和 Windows Server 2008 中添加

- SID: S-1-16-8448
  名称： 中加上强制性级别
  说明： 一个中型加上完整性级别。

  注意：Windows Vista 和 Windows Server 2008 中添加

- SID: S-1-16-12288
  名称： 高强制性级别
  说明： 高完整性级别。

  注意：Windows Vista 和 Windows Server 2008 中添加

- SID: S-1-16-16384
  名称： 系统强制性级别
  描述： 系统完整性级别。

  注意：Windows Vista 和 Windows Server 2008 中添加

- SID: S-1-16-20480
  名称： 保护进程强制性级别
  说明： 保护进程的完整性级别。

  注意：Windows Vista 和 Windows Server 2008 中添加

- SID: S-1-16-28672
  名称： 安全进程强制性级别
  说明： 安全进程完整性级别。

  注意：Windows Vista 和 Windows Server 2008 中添加

下面的组显示为 Sid，直到 Windows Server 2003 的域控制器是主域控制器 (PDC) 操作主机角色担任者。"操作主机"被也称为灵活的单主机操作 (FSMO)。Windows Server 2003 的域控制器添加到域，则会创建以下其他内置的组：

- SID: S-1-5-32-554
  名称： BUILTIN\Pre Windows 2000 以前版本兼容访问
  描述： Windows 2000 通过添加一个别名。向后兼容性组，从而允许所有用户和组的域中的读取访问权限。
- SID: S-1-5-32-555
  桌面机用户的名称： BUILTIN\Remote
  说明： 别名。此组中的成员被授予远程登录的权利。
- SID: S-1-5-32-556
  名称： BUILTIN\Network 配置操作员
  说明： 别名。此组中的成员可以有部分管理权限来管理网络功能的配置。
- SID: S-1-5-32-557
  名称： BUILTIN\Incoming 林信任构建器
  说明： 别名。此组的成员可以创建到此目录林的传入的单向信任。
- SID: S-1-5-32-558
  名称： BUILTIN\Performance 监视器用户
  说明： 别名。此组的成员可以远程访问以监视此计算机。
- SID: S-1-5-32-559
  名称： BUILTIN\Performance 日志用户
  说明： 别名。此组的成员可以远程访问以计划此计算机上性能计数器的日志。
- SID: S-1-5-32-560
  名称： BUILTIN\Windows 授权访问组
  说明： 别名。此组的成员具有对计算所得的 tokenGroupsGlobalAndUniversal 属性访问在用户对象上。
- SID: S-1-5-32-561
  名称： BUILTIN\Terminal 服务器许可证服务器
  说明： 别名。终端服务器许可证服务器组。如果安装 Windows 服务器 2003 Service Pack 1，创建新的本地组。
- SID: S-1-5-32-562
  名称： BUILTIN\Distributed COM 用户
  说明： 别名。COM 提供计算机范围的访问控制功能，控制访问所有的组调用，激活或启动计算机上的请求。

下面的组显示为 Sid，直到 Windows Server 2008 或 Windows Server 2008 R2 的域控制器是主域控制器 (PDC) 操作主机角色担任者。"操作主机"被也称为灵活的单主机操作 (FSMO)。Windows Server 2008 或 Windows Server 2008 R2 的域控制器添加到域，则会创建以下其他内置的组：

- SID: S 1 5 21-*域*-498
  名称： 企业只读域控制器
  说明： 将通用组。此组的成员企业中是只读域控制器
- SID: S 1 5 21-*域*-521
  只读的域控制器名称：
  说明： 一个全局组。此组的成员是域中的只读域控制器
- SID: S-1-5-32-569
  名称： BUILTIN\Cryptographic 运算符
  说明： 内置本地组。成员有权执行加密操作。
- SID: S 1 5 21-*域*-571
  名称： 允许 RODC 密码复制组
  说明： 域本地组。此组中的成员可以将密码复制到域中的所有只读域控制器。
- SID: S 1 5 21-*域*-572
  名称： 拒绝 RODC 密码复制组
  说明： 域本地组。此组中的成员的密码复制到域中的所有只读域控制器不能
- SID: S-1-5-32-573
  名称： BUILTIN\Event 日志读取器
  说明： 内置本地组。此组的成员可以从本地机器读取事件日志。
- SID: S-1-5-32-574
  名称： BUILTIN\Certificate 服务 DCOM 访问
  说明： 内置本地组。此组的成员可以在企业中连接到证书颁发机构。

下面的组显示为 Sid，直到 Windows Server 2012 域控制器是主域控制器 (PDC) 操作主机角色担任者。"操作主机"被也称为灵活的单主机操作 (FSMO)。Windows Server 2012 域控制器添加到域，则会创建以下其他内置的组：

- SID: S-1-5-21--522 的*域*
  克隆的域控制器名称：
  说明： 一个全局组。此组成员的域控制器可能被克隆。
- SID: S-1-5-32-575
  名称： BUILTIN\RDS 远程访问服务器
  说明： 内置本地组。此组中的服务器启用 RemoteApp 程序和个人虚拟机对这些资源的访问权限的用户。在面向 Internet 的部署中，这些服务器通常部署在边缘网络中。此组需要填充 RD 连接代理运行的服务器上。RD 网关服务器和远程桌面 Web 访问服务器部署中使用需要此组中。
- SID: S-1-5-32-576
  终结点的名称： BUILTIN\RDS 的服务器
  说明： 内置本地组。此组中的服务器运行用户 RemoteApp 程序和个人虚拟机的虚拟机和主机会话运行。此组需要填充 RD 连接代理运行的服务器上。RD 会话主机服务器和部署中使用 RD 虚拟化主机服务器需要此组中。
- SID: S-1-5-32-577
  名称： BUILTIN\RDS 管理服务器
  说明： 内置本地组。此组中的服务器可以运行远程桌面服务的服务器上执行日常的管理操作。此组需要远程桌面服务部署中的所有服务器上进行填充。运行 RDS 中央管理服务的服务器必须包含在此组中。
- SID: S-1-5-32-578
  名称： BUILTIN\Hyper V 管理员
  说明： 内置本地组。此组的成员拥有完全不受限制地访问所有功能的 Hyper-V。
- SID: S-1-5-32-579
  名称： BUILTIN\Access 控件帮助操作员
  说明： 内置本地组。授权特性和在此计算机上的资源的权限，这个组的成员可以远程查询。
- SID: S-1-5-32-580
  名称： BUILTIN\Remote 管理用户
  说明： 内置本地组。此组的成员可以访问 WMI 资源 （如 WS 管理通过 Windows 远程管理服务） 的管理协议。这仅适用于向用户授予访问权限的 WMI 命名空间。

参考链接：
http://www.cnblogs.com/awpatp/archive/2009/12/31/1636976.html
https://support.microsoft.com/zh-cn/help/243330/well-known-security-identifiers-in-windows-operating-systems
