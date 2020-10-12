---
description: Obtaining data for tournament questions
---

# Obtaining  Data

## Obtaining data for tournament questions

After a fair and transparent selection process, the topics chosen for the 2020 CHENDU80 FINTECH CONTEST is：

```
 chosen topic 
 
```

Participants can log in to the competition environment and read it directly by mounting it to their own online operating system, or they can get it by downloading it. 

The specific operation steps are as follows：

{% hint style="info" %}
**Mount S3** 

s3fs s3fs-mount-bucket /home/ec2-user/s3mnt -o passwd\_file=/home/ec2-user/.passwd-s3fs -o url=[http://s3.cn-north-1.amazonaws.com.cn](http://s3.cn-north-1.amazonaws.com.cn) -o endpoint=cn-north-1
{% endhint %}

\*\*\*\*

{% hint style="info" %}
 **Download**

\*\*\*\*[**install & config AWS CLI**](../service-documents/aws-cli.md)\*\*\*\*

aws s3 ls（find the bucket and file）

aws s3 cp s3://XXXX  /local/
{% endhint %}





