# Obtaining  Data

The competition data and competition questions are stored in the  "**fintech80chengdu-topic**"  S3 bucket, and you can get them in the following ways.

## 1. Log in to the AWS console and download relevant data from the S3 bucket.（ <mark style="color:red;">Not</mark> recommended, but  intuitive and simple）

1\)In the **Buckets** list, choose the bucket that you want to download objects.

2\)In the object list, check the object you want to download.

3\)Choose **Actions**, then choose **Download**.

4\)Choose “Download” In the **Download objects** dialog box.You've successfully downloaded an object from your bucket.

## 2. Download with AWS CLI command line.  (<mark style="color:red;">Recommended</mark>, support large files and intermittent transfer, fast speed）

#### [**install & config AWS CLI**](../../service-documents/aws-cli.md)

```
aws s3 ls（find the bucket and file）
```

![](<../../.gitbook/assets/image (99).png>)&#x20;

```
aws s3 cp s3://fintech80chengdu-topic /local/
```

![](../../.gitbook/assets/1603077877-1-.png)&#x20;

## &#x20;3. S3 browser(Windows)

{% hint style="info" %}
Detailed instructions are available on the [S3 browser ](https://s3browser.com/s3browser-first-run.aspx)
{% endhint %}

#### &#x20;[**install & config AWS CLI**](../../service-documents/aws-cli.md)

###
