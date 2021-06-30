# Obtaining  Data

## Obtaining data for the CHENGDU80-2020 Question

```text
 All data and questions are stored in the chengdu80-topic storage bucket.
```

Participants can log in to the competition environment and read it directly by mounting it to their own online operating system, or they can get it by downloading it.

The specific operation steps are as follows：

* [Download From S3](obtaining-data.md#download-from-s3)
* [Mount S3 as a disk](obtaining-data.md#mount-s3)

### **Download from S3**

{% hint style="info" %}
**Download**

\*\*\*\*[**install & config AWS CLI**](../../service-documents/aws-cli.md)\*\*\*\*

**aws s3 ls（find the bucket and file）**

\*\*\*\*![](../../.gitbook/assets/image%20%2899%29.png) _\*\*_

**aws s3 cp s3://chengdu80-project/XXX /local/**

\*\*\*\*![](../../.gitbook/assets/1603077877-1-.png) _\*\*_

for example:

**aws s3 cp s3://chengdu80-topic/topic1 ./root/**
{% endhint %}

If there are large files on the windows side that cannot be uploaded or downloaded, you can use the official free tool [S3 Browser](https://s3browser.com/download/s3browser-9-2-1.exe).

Install&open the S3 browser,click Account - Add New Account\(Fill in your account key information\)

![](../../.gitbook/assets/image-s3browser%20%281%29.jpg)

{% hint style="info" %}
Detailed instructions are available on the [S3 browser ](https://s3browser.com/s3browser-first-run.aspx)
{% endhint %}

### **Mount S3**

{% hint style="info" %}
**\(optional\)Mount S3**

**sudo apt-get（yum） update**

**sudo apt-get（yum） install git**

**git clone** [**https://github.com/s3fs-fuse/s3fs-fuse.git**](https://github.com/s3fs-fuse/s3fs-fuse.git)\*\*\*\*

**cd s3fs-fuse**

**./autogen.sh**

**./configure**

**make**

**sudo make install**

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

**s3fs bucket-name /path/to/mountpoint -o passwd\_file=/path/passwd-s3fs -o endpoint=ap-east-1**

In our example:

**s3fs chengdu80final-project ~/s3-bucket -o passwd\_file=~/.passwd-s3fs -o endpoint=ap-east-1**
{% endhint %}

