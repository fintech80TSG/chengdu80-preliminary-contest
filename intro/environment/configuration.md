# Configuration

Under the rule of fairness and justice, participants should compete in the environment provided, via the following steps:

* Connect to the designated network; 
* Connect to the designated servers\(EC2\) ; 
* Develop, deploy and demonstrate the project in the designated servers.

## 1. Architecture

Each team will be provided with two servers \(Windows 2016 or Ubuntu 18.04 or Centos7\).  Participants should develop and deploy under the given environment.   
All operations will be recorded.

![](../../.gitbook/assets/image%20%2893%29.png)

## 2.  EC2（Elastic Computer Cloud）

Each team will be provided with two EC2 servers.

The two EC2 can be configured as Windows operating system or Ubuntu/Centos operating system, but it should be **noted** that **the way to connect to the server varies according to the operating system of the terminal**.

Hardware configuration is as follows：

| CPU | RAM | HDD | OS |
| :--- | :--- | ---: | ---: |
| Xeon 8vCPU | 32GB | 200GB SSD | Windows10/Ubuntu 18.04/Centos7 |

{% hint style="info" %}
All teams in China will use servers in the Hong Kong region by default. We have optimized the connection from the cities to Hong Kong via the accelerator. Each team's accelerator provides 40GB of traffic by default \(which is enough for normal usage\), please contact technical support if you need more information. 
{% endhint %}

## **3.  Basic services**

The network for each team's servers is isolated from each other. There is 10 Gigabit bandwidth between aws servers.

To support the completion of the project, the following services are provided:

* [GIT ](../../operation-manual/competition-operation/code-submission.md) 
* [S3 bucket](../../service-documents/aws-s3.md)
* [Limit ](limit.md)
* [Backup ](../../operation-manual/competition-operation/backup-and-restore.md)



