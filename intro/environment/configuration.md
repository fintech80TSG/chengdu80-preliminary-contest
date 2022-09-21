# Configuration

## 1. EC2（Elastic Computer Cloud）

### 1.1  EC2 resource

Each team will be provided with two EC2 servers.

The two EC2 can be configured as Windows operating system or Ubuntu/Centos operating system, but it should be **noted** that **the way to connect to the server varies according to the operating system of the terminal**.

Hardware configuration is as follows：

| CPU        | RAM  |       HDD |                             OS |
| ---------- | ---- | --------: | -----------------------------: |
| Xeon 8vCPU | 32GB | 200GB SSD | Windows10/Ubuntu 18.04/Centos7 |

{% hint style="info" %}
All teams in China will use servers in the Hong Kong region by default. We have optimized the connection from the cities to Hong Kong via the accelerator. Each team's accelerator provides 40GB of traffic by default (which is enough for normal usage), please contact technical support if you need more information.
{% endhint %}

### 1.2 EC2 resource limit

We limited each participating team can only use 2 EC2 Server. (3 select 2)

Windows Server 2016 R2

Ubuntu 18.04

Centos 7

Each team can only operate its own resources，can start/stop/restart your team

{% hint style="danger" %}
Warning: Don't touch other teams resource,and you have not permission to create new instances.
{% endhint %}

## 2. S3（Simple Storage Service）

Each team only has upload and download permissions for their own team's named folders, but neither can download or delete content uploaded by other teams.

If your team need additional S3 bucket, plz [Contact us.](../../tech-support/online-support.md)

## 3. Limit Security Groups(Ports)

Each EC2 Server will only open limit Ports 60-9000.You should start your server on these Ports.If your team need special ports,plz [Contact us.](../../tech-support/online-support.md)

## **4. Basic services**

The network for each team's servers is isolated from each other. There is 5 Gigabit bandwidth between aws servers.

To support the completion of the project, the following services are provided:

* [GIT ](../../operation-manual/steps/competition-operation/code-submission.md)&#x20;
* [Backup ](../../operation-manual/steps/competition-operation/backup-and-restore.md)

## 5. Prohibited content

It is prohibited to submit any content irrelevant to the event of CHENG80. If any illegal or illegal controversial content is involved, the event party will hold responsible.
