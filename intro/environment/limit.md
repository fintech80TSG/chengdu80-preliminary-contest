# Limits

In addition to the following technical constraints, we require teams to：

* Prohibit the use of computing resources for non-competition-related content 
* Prohibit the use of computing resources to publish any content not related to the competition 
* It is forbidden to post non-competition related content on the Teams platform. 
* Don't leak the questions and data of the contest.



### 3.1 Limit resources

We limited each participating team can only use 2 EC2 Server. \(3 select 2\)

* [ ] Windows Server 2016R2
* [ ] Ubuntu 18.04
* [x] Centos 7

Each team can only operate its own resources，can start/stop/restart your team

{% hint style="danger" %}
Warning: Don't touch other teams resource,and you have not permission to create new instances.
{% endhint %}

### 3.2 Limit S3

Each team only has upload and download permissions for their own team's named folders, but neither can download or delete content uploaded by other teams.

If your team need additional S3 bucket, plz [Contact us.](../../tech-support/online-support.md)

### 3.3 Limit  Security Groups\(Ports\)

Each EC2 Server will only open limit Ports  60-9000.You should start your server on these Ports.If your team need special ports,plz [Contact us.](../../tech-support/online-support.md)

### 3.4 Prohibited content

It is prohibited to submit any content irrelevant to the event of CHENG80. If any illegal or illegal controversial content is involved, the event party will hold responsible.

