# 网络空间的理解和特点

网络空间包含以下 4 种组成要素：

- 载体
- 资源
- 主体
- 操作

网络空间可以被定义为：构建在信息通信技术基础上的人造空间，用以支撑人们在该空间中开展各类与信息通信技术相关的活动。

## 特点：

- 网络空间是一个和海陆空并存的“域”。
- 网络空间环境下，计算机系统设计的软硬件组成更广泛，结构层次更复杂，承载的信息更丰富，系统和环境的交互更密切，信息内容的传播影响更深远。
- 在网络空间中，通过对信息的控制，可以实现对物理信息系统的操控，从而影响人的认知和活动。
- 网络空间是由人，机 ，物相互作用形成的动态虚拟空间，不仅仅包含传统互联网依托的各类电子设备，人也是构成网络空间的重要元素。
- 网络空间作为新的“全球公共空间”，被视为陆海空天之外的”第五空间“。是一个新型军事空间、外交空间和意识形态空间，具有鲜明的主权特征。

# 信息安全的定义

很难对信息安全给出一个完整的定义，但可以从反面罗列出一些不安全的情况，例如：

- 系统不及时打补丁。
- 使用弱口令。
- 随意从网络下载应用程序。
- 打开陌生用户的电子邮件附件。
- 使用不加密的无线网络。

## 信息安全脆弱点

信息安全脆弱点划分为以下两种：

### 技术脆弱点

包括物理环境，软件系统，网络和通信协议等。

### 管理脆弱点

包括管理组织，管理制度，管理执行等。

## CIA 安全需求模型

CIA 的概念如下所示：

- C：保密性（Confidentiality）
- I：完整性（Integrity）
- A：可用性（Availability）

## 信息安全防护的发展

- 信息保密阶段。
- 网络信息安全阶段。
- 信息保障阶段。

保障阶段提出了PDRR模型，它是保护（Protection）、检测（Detection）、响应（Reaction）、恢复（Restore）的有机结合。

## 信息安全防护的基本原则

- 整体性原则（木桶理论）。
- 分层性原则。
- 旁路攻击。

### 需要掌握概念

旁路攻击指攻击者通过偷窥，分析敲击键盘的声音等手段来在不设防的设备区域获取一定的信息，是一种利用计算机或其他电子设备在运行时产生的物理效应来获取设备内部信息的攻击方式。

常见的旁路攻击手段：溢出攻击。

## 密码体制的基本组成

密码体制通过以下成分组成：

- 明文
- 密文
- 加密
- 解密
- 密钥

## 常见密码攻击方法

- 穷举攻击
- 统计分析攻击
- 数学分析攻击
- 社会工程攻击
- 针对密码算法的侧信道攻击

## 分组密码

分组密码又叫块密码，是将明文数据分成多个等长的数据块，对每个块以同样的密钥和同样的处理过程进行加密或解密。

### 常见对称密码算法

- DES：分组长度64位，密钥长度56位。
- 3-DES：密钥长度168位。
- AES：分组长度128位，密钥长度可变（128/192/256）。

### 常见公钥密码算法

- RSA

## 哈希函数的概念

哈希函数可以把满足要求的任意长度的输入转换为固定长度的输出，是一种单向密码体制，只有加密，不能解密。

### 哈希函数的应用

- 校验数据完整性。
- 数字签名。
- 消息认证。
- 保护用户口令。
- 区块链。

### 常用哈希函数

- MD5对于任意长度的输入消息产生128位长度的哈希值。
- SHA-1算法输出一个160位的哈希值。

## 数字签名

数字签名是电子形式签名，具有以下特点：

- 不可否认。
- 不可伪造。
- 可认证。

## 信息隐藏

信息隐藏指将机密信息秘密隐藏于另一公开的信息（称为载体），然后将其通过公开通道来传递。

### 信息隐藏技术的基本要求

- 鲁棒性：载体受到某种扰动也能恢复隐藏信息。
- 不可感知性。
- 安全性。
- 信息量。

## 身份认证的概念

身份认证是证实实体对象的数字身份与物理身份是否一致的过程，这里的实体可以是用户也可以是主机系统。

身份认证分为两个过程：标识和鉴别。

### 身份凭证信息

常用的身份凭证信息如下：

- 用户所知道的：用户记忆的口令，密钥等。
- 用户所拥有的：用户的物理识别设备。
- 用户本身的特征：用户的生理特征。

## 一次性口令的基本原理

在登录过程中加入不确定因子，使用户在每次登录时产生的口令信息都不相同。

## 公钥基础设施PKI

PKI 是一种用于管理数字证书的体系结构。

PKI 的本质是实现大规模网络中的信任基础。它提供了一整套安全机制，使用户在不知道对方身份或分布地点的情况下，以数字证书为基础，通过一系列的信任关系进行网络通信和网络交易。

### 认证中心CA

CA是PKI中存储、管理、发布数字证书的可信机构或服务器。当用户请求生成证书时，注册授权中心验证用户的身份并将用户的请求发送给CA，CA会创建证书，签名，并在证书的有效期内管理证书。

### PKI应用实例

以PKI为基础的安全应用非常多，PKI技术可以保障Web交易多方面的安全需求，使Web上的交易和面对面的交易一样安全。

### 为什么需要可信第三方CA？

如果不存在认证机构，任何人都可以制作数字证书，网络中的两个实体进行信息交互就可能被中间人攻击。

### 谁能成为认证授权中心CA？

- 依法成立的合法组织。
- 具有与认证服务相适应的专业技术人员和管理人员。
- 具有与提供认证服务相适应的资金和场所，具备提供认证服务和承担风险责任的能力。
- 具有符合国家安全标准的技术、设备。
- 国家法律法规规定的其他条件。

## 威胁操作系统安全的因素

- 硬件设备。
- 环境因素。
- 网络攻击破坏系统的保密性、完整性和可用性。
- 隐蔽信道破坏系统的保密性和完整性。
- 用户的误操作破坏系统的可用性和完整性。
- 不断被发现的系统漏洞为安全事件的发生提供了可能。

## 操作系统的安全目标

操作系统安全是指操作系统在基本功能的基础上增加了安全机制和措施。

安全目标包括以下几个要点：

- 标识系统中的用户并进行身份鉴别。
- 依据系统安全策略对用户的操作进行访问控制。
- 监督系统运行的安全。
- 保证系统自身的安全性和完整性。

## 操作系统的安全机制

- 用户认证。
- 访问控制。
- 最小权限管理。
- 信道保护。
- 硬件保护。
- 文件系统保护。
- 安全审计。

## 什么是Windwos操作系统最小权限原则

默认以普通用户的身份执行操作，只有在权限不足的情况下才会使用管理员身份。

## 数据库系统安全的重要性

- 包含敏感数据和信息资产。
- 是计算机信息系统安全的关键环节。

## 数据库的安全机制

- 用户认证。
- 用户授权。
- 角色管理。
- 访问控制。
- 安全审计。
- 备份恢复。
- 数据加密。
- 资源限制。

## 网络攻击的基本步骤

- 隐藏攻击源。
- 信息搜集。
- 掌握系统控制权。
- 实施攻击。
- 安装后门。
- 清除攻击痕迹。

## 网络攻击的常用手段

- 伪装攻击。
- 探测攻击。
- 嗅探攻击。
- 解码类攻击。
- 缓冲区溢出攻击。
- 欺骗攻击。
- 拒绝服务攻击。
- Web脚本入侵。
- 0day攻击。
- 社会工程学攻击。

## APT的定义

- A：技术高级。
- P：持续时间长。
- T：威胁性大。

## APT攻击的一般过程

- 信息侦察。
- 持续渗透。
- 长期潜伏。
- 窃取信息。

## APT攻击与传统攻击的比较

攻击者为资金充足、有组织、有背景的黑客团队。		

目标对象是国家重要基础设施，重点组织和人物。

目标数据是价值很高的电子资产，如国家安全数据、商业机密等。

目的是提升国家的战略优势，操纵市场，摧毁关键设施等。

## TCP/IPv4的脆弱性

TCP/IPv4普遍缺少安全机制，因为协议设计者主要关注于网络运行和应用相关的技术问题，安全问题考虑甚少。

## 防火墙的分类

按照防火墙产品的形态，可以分为软件防火墙和硬件防火墙。

## 防火墙技术原理

- 包过滤技术。
- 状态包过滤技术。

## 网络结构安全区域

- 外部网络。
- DMZ网络：隔离区。
- 内部网络：防火墙要保护的对象。

## 软件漏洞

软件漏洞是软件系统或产品在设计、实现、配置、运行过程中，由操作实体有意或无意产生的缺陷、瑕疵或错误。

- 0day漏洞：已被发现但官方还没有相关补丁的漏洞。
- 1day漏洞：发布补丁后大部分用户还未打补丁的漏洞。

## SQL注入漏洞

攻击者将恶意代码插入查询语句或命令中，从而执行设计者预料外的操作。

## 恶意代码

恶意代码是在未授权的情况下，以破坏软硬件设备设备、窃取用户信息，干扰用户正常使用，扰乱用户心理为目的编写的软件或代码片段。

## 计算机病毒

指编制或者在计算机程序中插入的破坏计算机功能或毁坏数据，影响计算机使用，并能自我复制的一组计算机指令或程序代码。

## 蠕虫

主动扫描和攻击网络上存在系统漏洞的节点主机，通过网络从一个节点传播到下一个节点。

## 软件逆向工程

软件逆向工程指通过分析目标软件的二进制代码，来了解它的内部结构、功能和算法的一种技术。

## 软件知识产权

按照国际惯例，知识产权主要通过版权（著作权）进行保护。

## 软件版权保护的技术保护目标和基本原则

软件版权保护旨在保护某个特定的计算机程序以及程序中所包含信息的完整性、保密性和可用性。

## 信息内容安全的目标

- 可控性。
- 保密性和可追溯性。
- 可用性。

## 知识产权保护技术

知识产权包括专利权、商标权、版权、商业秘密等类型。
