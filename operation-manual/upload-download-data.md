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

 sudo apt-get（yum） update

 sudo apt-get（yum） install s3fs

 echo ACCESS\_KEY:SECRET\_ACCESS\_KEY &gt; PATH\_TO\_FILE

（Access\_key/Secret\_access\_key will send with account password to your email）

 cat ~/.passwd-s3fs

 chmod 600 ~/.passwd-s3fs

 mkdir ~/s3-bucket

 s3fs bucket-name /path/to/mountpoint -o passwd\_file=/path/passwd-s3fs
{% endhint %}

\*\*\*\*

{% hint style="info" %}
 **Download**

\*\*\*\*[**install & config AWS CLI**](../service-documents/aws-cli.md)\*\*\*\*

aws s3 ls（find the bucket and file）

aws s3 cp s3://XXXX  /local/
{% endhint %}





