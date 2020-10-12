# Configuration

### 1. Architecture

Under the rule of fairness and justice, participants should compete in the environment provided, via the following steps: 

* Connect to the designated network; 
* Connect to the designated servers through the login server; 
* Develop, deploy and demonstrate the project in the designated servers.

 Each team will be provided with  two virtual servers \(Windows 2016 or Ubuntu 18.04 or Centos7\). Contestants could also bring their own devices to the site. Participants should develop and deploy under the given environment. All operations will be audited and recorded.

![](../../.gitbook/assets/image%20%2867%29.png)

### 2.  EC2（Elastic Computer Cloud）

Each team will be provided  with two EC2.

The two EC2 can be configured as Windows operating system or Ubuntu/Centos operating system, but it should be **noted** that **the way to connect to the server varies according to the operating system of the terminal**.

Hardware configuration is as follows：

| CPU | RAM | HDD | Ethernet | OS |
| :--- | :--- | ---: | ---: | ---: |
| Xeon 4vCPU | 16GB | 200GB SSD | 10Gbps | Windows10/Ubuntu 18.04/Centos7 |

{% hint style="info" %}
As there will be network problems for Chinese participating teams to log in EC2 overseas, we will provide acceleration service\(GA\) for Chinese teams to speed up to Hong Kong to ensure the stability of login.each team can get 40GB data transfer ,If your team want to apply more, please [Connect us](../../tech-support/online-support.md).
{% endhint %}



### **3.  Basic services**

The network for each team's servers is isolated from each other. There is 10 Gigabit bandwidth between the two given servers, and Gigabit bandwidth between terminals and servers. 

To support the completion of the project, the following services are provided:

* GIT  
* [S3 bucket](../../service-documents/aws-s3.md)
* [Limit ](limit.md)
* [Backup](../../operation-manual/develops-and-backup.md) 



