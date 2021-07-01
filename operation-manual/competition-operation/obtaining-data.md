# Obtaining  Data

## Obtaining data for the CHENGDU80-2020 Question

赛事数据和题目都存储在s3chengdu80-topic存储桶中，您可以通过以下方式获取

1. aws控制台网页下载，操作参考...

    2. aws cli 命令行下载

[**install & config AWS CLI**](../../service-documents/aws-cli.md)

```text
aws s3 ls（find the bucket and file）
```

![](../../.gitbook/assets/image%20%2899%29.png) 

```text
aws s3 cp s3://chengdu80-project/XXX /local/
```

![](../../.gitbook/assets/1603077877-1-.png) 

```text
aws s3 cp s3://chengdu80-topic/topic1 ./root/
```

    3. s3 browser\(Windows\)

{% hint style="info" %}
Detailed instructions are available on the [S3 browser ](https://s3browser.com/s3browser-first-run.aspx)
{% endhint %}

 4. 挂载 s3 到系统目录\(Linux\)

[**install & config AWS CLI**](../../service-documents/aws-cli.md)

安装 goofys

```text
wget https://github.com/kahing/goofys/releases/latest/download/goofys
chmod +x goofys
sudo mv goofys /usr/local/bin/
// centos
sudo yum install -y fuse
// ubuntu
sudo apt install fuse
```

挂载 S3

```text
sudo mkdir -p /Mount-Point （挂载文件夹）
sudo chown Your-User-Name:Your-User-Name （系统用户名，如：centos） /Mount-Point
/usr/local/bin/goofys Your-Bucket:Your-School-Prefix （大学简称） /Mount-Point
```

