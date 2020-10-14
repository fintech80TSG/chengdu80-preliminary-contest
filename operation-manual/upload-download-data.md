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

 **sudo apt-get（yum） update**

 **sudo apt-get（yum） install s3fs**

 **echo ACCESS\_KEY:SECRET\_ACCESS\_KEY &gt; PATH\_TO\_FILE**

（Access\_key/Secret\_access\_key will send with account password to your email,Path\_to\_file is new key file）

for example:

 **echo AKIA4SK3HPQ9FLWO8AMB:esrhLH4m1Da+3fJoU5xet1/ivsZ+Pay73BcSnzP &gt; ~/.passwd-s3fs**

Check whether the keys were written to the file:

 **cat ~/.passwd-s3fs**

Set correct permissions for the _passwd-s3fs_ file where the access keys are stored:

 **chmod 600 ~/.passwd-s3fs**

Create the directory \(mount point\) that will be used as a mount point for your S3 bucket. In this example, we create the Amazon cloud drive S3 directory in the home user’s directory:

 **mkdir ~/s3-bucket**

now we can mount aws s3:

 **s3fs bucket-name /path/to/mountpoint -o passwd\_file=/path/passwd-s3fs**

In our example:

 **s3fs chengdu80final-project ~/s3-bucket -o passwd\_file=~/.passwd-s3fs**
{% endhint %}

\*\*\*\*

{% hint style="info" %}
 **Upload**

\*\*\*\*[**install & config AWS CLI**](../service-documents/aws-cli.md)\*\*\*\*

**aws s3 ls（find the bucket and file）**

**aws s3 cp /local/ s3://chengdu80final-project/XXX**

for example:

**aws s3 cp ./root/ s3://chengdu80final-project/topic1**
{% endhint %}

\*\*\*\*

{% hint style="info" %}
 **Download**

\*\*\*\*[**install & config AWS CLI**](../service-documents/aws-cli.md)\*\*\*\*

**aws s3 ls（find the bucket and file）**

**aws s3 cp s3://chengdu80final-project/XXX  /local/**

for example:

**aws s3 cp s3://chengdu80final-project/topic1 ./root/**
{% endhint %}





