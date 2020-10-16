# Environment Test

Test your environment according to the following test steps .

## 3.1 Test connection to EC2

{% hint style="warning" %}
Due to regional restrictions, the server addresses of the following teams are **different \(Using** [**GA service**](https://aws.amazon.com/cn/global-accelerator/?blogs-global-accelerator.sort-by=item.additionalFields.createdDate&blogs-global-accelerator.sort-order=desc&aws-global-accelerator-wn.sort-by=item.additionalFields.postDateTime&aws-global-accelerator-wn.sort-order=desc)**\),** so emailed account information should be noted.   
  
It is recommended that you use the connection information provided by mail.  
  
Tsinghua University/THU   
Southern University of Science and Technology /SUSTech Chongqing University/CQU   
Southwestern University of Finance and Economics/SWUFE\)
{% endhint %}

**1.Connect to Centos7 or Ubuntu18.04 LTS**

**Connect using PuTTY** 

a. Download and install PuTTY from the [PuTTY download page](http://www.chiark.greenend.org.uk/~sgtatham/putty/). 

b.Start PuTTY \(from the **Start** menu, choose **All Programs, PuTTY, PuTTY**\).

c.In the **Category** pane, choose **Session** and complete the following fields:

1. run puttygen.exe,load `.pem`file change to`.ppk` file.
2. In the **Host Name** box: public ip\(ipv4\).
3. In the **Port Name** box: 22
4. Select **Connection** -&gt; **SSH** -&gt; **Auth**,browse the `.ppk` file.

![](../.gitbook/assets/image%20%2885%29.png)

    5.Click **Open**.

{% hint style="info" %}
 \(Optional\) You can configure PuTTY to automatically send 'keepalive' data at regular intervals to keep the session active. This is useful to avoid disconnecting from your instance due to session inactivity. In the **Category** pane, choose **Connection**, and then enter the required interval in the **Seconds between keepalives** field. For example, if your session disconnects after 10 minutes of inactivity, enter 180 to configure PuTTY to send keepalive data every 3 minutes.
{% endhint %}

Other SSH client please find the information about [SSH Client](https://www.slant.co/topics/149/~best-ssh-clients-for-windows).

**2.Connect to Windows 2016 R2**

a.Open the Amazon EC2 console at [https://console.aws.amazon.com/ec2/](https://console.aws.amazon.com/ec2/).

b.Choose **EC2** enter the Page.

c.Choose **Get Windows password**. 

![](../.gitbook/assets/image%20%2878%29.png)

d.Select the file name of the private key \(`.pem`\) and unzip.

![](../.gitbook/assets/image%20%2875%29.png)

![](../.gitbook/assets/image%20%2874%29.png)

e.Copy **Password**.

![](../.gitbook/assets/image%20%2876%29.png)

f.Using Windows mstsc\(Remote Desktop Connection\) to connect.

![](../.gitbook/assets/image%20%2860%29.png)

g.Enter the **default user name** and **Password**.

![](../.gitbook/assets/image%20%2863%29.png)

## 3.2 Test EC2 environment,

**1.Use EC2 to test the network speed \(for example: ping the local IP to test the delay\).**

2.**Check whether the EC2 environment meets the operating requirements of your data.**

## 3.3 Test S3 Upload/Download

**Open the Amazon S3 console at Services.**

![](../.gitbook/assets/image%20%2886%29.png)

1**.Uploading an object to a bucket**

1. In the **Bucket** list, choose the name of the bucket that you want to upload your object to.
2. On the **Overview** tab for your bucket, choose **Upload** or **Get Started**.
3. To choose the file to upload, in the **Upload** dialog box, choose **Add files**.
4. Choose a file to upload, and then choose **Open.**
5. Choose **Upload**.

You've successfully uploaded an object to your bucket.

**2.Delecting an object**

1. In the **Buckets** list, choose the name of the bucket that you want to delete an object from.
2. In the **Name** list, select the check box for the object that you want to delete.
3. Choose **Actions**, and then choose **Delete**.
4. In the **Delete objects** dialog box, verify the name of the object, and choose **Delete**.

You've successfully deleted an object to your bucket.

**3.Downloading an object from a bucket**

1. In the **Buckets** list, choose the name of the bucket that you want to download an object from.
2. In the **Name** list, select the check box for the object that you want to download.
3. Choose **Actions**, and then choose **Download**.
4. In the **Download objects** dialog box and choose **Download**.

You've successfully downloaded an object to your bucket.

## 3.4 Feedback usage













