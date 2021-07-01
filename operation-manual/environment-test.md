# Environment Test

In the pre-match testing session,  you need to do the following tests. 

1. verify if the aws console login is working properly and if the team introduction video can be uploaded via S3. 

2. check whether the server operating system is correct and whether it can be logged on normally 

3. verify that the connection speed to the server is normal and that there is no lag.

## Connect to EC2

### 1.select Services -&gt; EC2 buttons

![](../.gitbook/assets/image%20%287%29.png)

### 2.get EC2 information

![](../.gitbook/assets/image%20%284%29.png)

{% hint style="warning" %}
由于地域限制，中国大陆的参赛团队的服务器地址不同，请注意查阅邮件里的加速地址信息， 建议您使用邮件提供的IP地址。
{% endhint %}

## Connect to Operating System

### 1.Connect to Linux

#### **1.1 Windows Connect to Centos7 or Ubuntu18.04 LTS**

\(Note:PuTTY is not a designated SSH tool, other login methods are allowed\)

Connect using PuTTY

\(1\).Download and install PuTTY from the [PuTTY download page](http://www.chiark.greenend.org.uk/~sgtatham/putty/).

\(2\).Start PuTTY \(from the Start menu, choose All Programs, PuTTY, PuTTY\).

\(3\).In the Category pane, choose Session and complete the following fields:

\(4\).run puttygen.exe,load `.pem`file change to`.ppk` file.

* From the Start menu, choose All Programs, PuTTY, PuTTYgen.
* Under Type of key to generate, choose RSA. If you're using an older version of PuTTYgen, choose SSH-2 RSA.

![](../.gitbook/assets/image%20%288%29.png)

* Choose Load. By default, PuTTYgen displays only files with the extension `.ppk`. To locate your `.pem` file, choose the option to display files of all types.

![](../.gitbook/assets/image%20%282%29.png)

* Select your `.pem` file for the key pair that you specified when you launched your instance and choose Open. PuTTYgen displays a notice that the `.pem` file was successfully imported. Choose OK.
* To save the key in the format that PuTTY can use, choose Save private key. PuTTYgen displays a warning about saving the key without a passphrase. Choose Yes.

  \(5\). In the Host Name box: public ip\(ipv4\).

  \(6\). In the Port Name box: 22

  \(7\).Select Connection -&gt; SSH -&gt; Auth,browse the `.ppk` file.

![](../.gitbook/assets/image%20%2885%29.png)

{% hint style="info" %}
\(Optional\) You can configure PuTTY to automatically send 'keepalive' data at regular intervals to keep the session active. This is useful to avoid disconnecting from your instance due to session inactivity. In the **Category** pane, choose **Connection**, and then enter the required interval in the **Seconds between keepalives** field. For example, if your session disconnects after 10 minutes of inactivity, enter 180 to configure PuTTY to send keepalive data every 3 minutes.
{% endhint %}

Other SSH client please find the information about [SSH Client](https://www.slant.co/topics/149/~best-ssh-clients-for-windows).

#### **1.2 MAC Connect to Linux**

1.open the terminal

![](../.gitbook/assets/image%20%28106%29.png)

2.Input the command: ssh -i _key_.pem _username_@_host_

for example:

![](../.gitbook/assets/image%20%28103%29.png)

### **2.Connect to Windows** 

2.1 Open the Amazon EC2 console at [https://console.aws.amazon.com/ec2/](https://console.aws.amazon.com/ec2/).

2.2 Choose EC2 enter the Page.

2.3 Choose Get Windows password.

![](../.gitbook/assets/image%20%2878%29.png)

2.4 Select the file name of the private key \(`.pem`\) and unzip.

![](../.gitbook/assets/image%20%2875%29.png)

![](../.gitbook/assets/image%20%2874%29.png)

2.5 Copy Password.

![](../.gitbook/assets/image%20%2876%29.png)

2.6 Using Windows mstsc\(Remote Desktop Connection\) to connect.

![](../.gitbook/assets/image%20%2860%29.png)

2.7 Enter the default user name and Password.

![](../.gitbook/assets/image%20%2863%29.png)

{% hint style="info" %}
MAC login:[https://remotedesktopmanager.com/](https://remotedesktopmanager.com/)
{% endhint %}

## Test EC2 environment

1.Test the network speed \(for example: ping the EC2 IP to test the delay\).

2.Check the EC2 environment \(OS etc\).

{% hint style="info" %}
Pre-install software is not allowed during the test session.
{% endhint %}

## Test file uploads and downloads in S3

Open the Amazon S3 console at Services.

![](../.gitbook/assets/image%20%2886%29.png)

**1.Uploading an object to a bucket**

1. In the **Bucket** list, choose the name of the bucket that you want to upload your object to.
2. Click the **Overview** tab for your bucket, choose **Upload** or **Get Started**.
3. To choose the file to upload, in the **Upload** dialog box, choose **Add files**.
4. Choose a file to upload, and then choose **Open.**
5. Choose **Upload**.

You've successfully uploaded an object to your bucket.

**2.Deleting an object**

1. In the **Buckets** list, choose the bucket that you want to delete objects.
2. In the **Name** list, select the check box for the object that you want to delete.在对象列表中，勾选要删除的对象。
3. Choose **Actions**, and then choose “Delete ”.
4.  Confirm the object that you want to delete in the Delete objects dialog box, then select “Delete ”.

    You've successfully deleted an object from your bucket.

**3.Downloading an object from a bucket**

1. In the **Buckets** list, choose the bucket that you want to download objects.
2. In the **Name** list, select the check box for the object that you want to download.在对象列表中，选中要下载的对象。
3. Choose **Actions**, then choose **Download**.
4. Choose “Download” In the **Download objects** dialog box.

     You've successfully downloaded an object from your bucket.

## Feedback usage

When you have completed the test,  please feedback us [the corresponding test results](https://forms.office.com/Pages/DesignPage.aspx?fragment=FormId%3DS8fgZBcaAECBySjMd29sdbARWGwIoxVBvYOnmX6MKMNUQUIwNEQ3SDE2UDJDOEE5MThEVllLTFpRUC4u).

