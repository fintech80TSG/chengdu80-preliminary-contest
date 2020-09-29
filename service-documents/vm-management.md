# 虚拟机管理

**Linux:**

**Linux有**[**不同登录方式**](https://docs.aws.amazon.com/zh_cn/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html%20)**，选择一种方式SSH登录。**

注：每个 Linux 实例均使用默认 Linux 系统用户账户启动。默认用户名由启动实例时指定的 AMI 决定。

`对于 Amazon Linux 2 或 Amazon Linux AMI，用户名称是 ec2-user。`

`对于 CentOS AMI，用户名称是 centos。`

`对于 Debian AMI，用户名称是 admin。`

`对于 Fedora AMI，用户名为 ec2-user 或 fedora。`

`对于 RHEL AMI，用户名称是 ec2-user 或 root。`

`对于 SUSE AMI，用户名称是 ec2-user 或 root。`

`对于 Ubuntu AMI，用户名称是 ubuntu。`

**Windows:**

在EC2实例控制台选中所要登录的Windows机器，点击**连接。**

![](../.gitbook/assets/image%20%2817%29.png)

点击弹框中的**获取密码。**

\*\*\*\*

![&#x9009;&#x62E9;&#x83B7;&#x53D6;&#x5BC6;&#x7801;&#x6309;&#x94AE;](../.gitbook/assets/image%20%282%29.png)

根据创建时所选带**.pem**的密钥，在**浏览**中找到放置在本地的密钥文件，通过该密钥**解压密码**。

![&#x627E;&#x5230;&#x5BC6;&#x94A5;&#x8DEF;&#x5F84;&#x4E0A;&#x4F20;](../.gitbook/assets/image%20%281%29.png)

![&#x89E3;&#x538B;&#x5BC6;&#x94A5;&#x83B7;&#x5F97;&#x5BC6;&#x7801;](../.gitbook/assets/image%20%284%29.png)

![&#x70B9;&#x51FB;&#x590D;&#x5236;&#x5BC6;&#x7801;](../.gitbook/assets/image%20%288%29.png)

用windows自带的远程连接去连，公网IP在EC2实例控制台上可查看。

![&#x67E5;&#x627E;EC2&#x516C;&#x7F51;ip](../.gitbook/assets/image%20%283%29.png)

![&#x4F7F;&#x7528;window&#x8FDC;&#x7A0B;&#x8FDE;&#x63A5;](../.gitbook/assets/image.png)

输入**公网IP**，**账户**，**密码**进行windows远程登录（windows默认账户为**Administrator**）。

![&#x8F93;&#x5165;&#x8D26;&#x6237;&#x5BC6;&#x7801;](../.gitbook/assets/image%20%286%29.png)

登录完成

![&#x767B;&#x5F55;&#x6210;&#x529F;&#x754C;&#x9762;](../.gitbook/assets/image%20%289%29.png)

