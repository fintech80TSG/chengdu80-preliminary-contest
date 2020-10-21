# Connect to EC2

How to connect to EC2 after we get public ip and key of EC2?

{% hint style="warning" %}
Due to regional restrictions, the server addresses of the following teams are **different \(Using** [**GA service**](https://aws.amazon.com/cn/global-accelerator/?blogs-global-accelerator.sort-by=item.additionalFields.createdDate&blogs-global-accelerator.sort-order=desc&aws-global-accelerator-wn.sort-by=item.additionalFields.postDateTime&aws-global-accelerator-wn.sort-order=desc)**\),** so emailed account information should be noted.   
  
It is recommended that you use the connection information provided by mail.  
  
Tsinghua University/ THU   
Southern University of Science and Technology / SUSTech   
Chongqing University/ CQU   
Southwestern University of Finance and Economics/ SWUFE  
University of Electronic Science and Technology of China /UESTC
{% endhint %}

## **Connect to Centos7 or Ubuntu18.04 LTS** <a id="PuttingAnObjectInABucket"></a>

**Connect using PuTTY** 

a. Download and install PuTTY from the [PuTTY download page](http://www.chiark.greenend.org.uk/~sgtatham/putty/). 

b.Start PuTTY \(from the **Start** menu, choose **All Programs, PuTTY, PuTTY**\).

c.In the **Category** pane, choose **Session** and complete the following fields:

a.run puttygen.exe,load `.pem`file change to`.ppk` file.

* From the **Start** menu, choose **All Programs**, **PuTTY**, **PuTTYgen**.
* Under **Type of key to generate**, choose **RSA**. If you're using an older version of PuTTYgen, choose **SSH-2 RSA**.

                                  ![
							RSA key in PuTTYgen
						](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/images/puttygen-key-type.png)

* Choose **Load**. By default, PuTTYgen displays only files with the extension `.ppk`. To locate your `.pem` file, choose the option to display files of all types. 

                                  ![
							Select all file types
						](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/images/puttygen-load-key.png)

* Select your `.pem` file for the key pair that you specified when you launched your instance and choose **Open**. PuTTYgen displays a notice that the `.pem` file was successfully imported. Choose **OK**.
* To save the key in the format that PuTTY can use, choose **Save private key**. PuTTYgen displays a warning about saving the key without a passphrase. Choose **Yes**.

b.In the **Host Name** box: public ip\(ipv4\).

c.In the **Port Name** box: 22

d.Select **Connection** -&gt; **SSH** -&gt; **Auth**,browse the `.ppk` file.

![](../../.gitbook/assets/image%20%2885%29.png)

    e.Click **Open**.

{% hint style="info" %}
 \(Optional\) You can configure PuTTY to automatically send 'keepalive' data at regular intervals to keep the session active. This is useful to avoid disconnecting from your instance due to session inactivity. In the **Category** pane, choose **Connection**, and then enter the required interval in the **Seconds between keepalives** field. For example, if your session disconnects after 10 minutes of inactivity, enter 180 to configure PuTTY to send keepalive data every 3 minutes.
{% endhint %}

Other SSH client please find the information about [SSH Client](https://www.slant.co/topics/149/~best-ssh-clients-for-windows).

## **Connect to Windows 2016 R2** <a id="PuttingAnObjectInABucket"></a>

a.Open the Amazon EC2 console at [https://console.aws.amazon.com/ec2/](https://console.aws.amazon.com/ec2/).

b.Choose **EC2** enter the Page.

c.Choose **Get Windows password**. 

![](../../.gitbook/assets/image%20%2878%29.png)

d.Select the file name of the private key \(`.pem`\) and unzip.

![](../../.gitbook/assets/image%20%2875%29.png)

![](../../.gitbook/assets/image%20%2874%29.png)

e.Copy **Password**.

![](../../.gitbook/assets/image%20%2876%29.png)

f.Using Windows mstsc\(Remote Desktop Connection\) to connect.

![](../../.gitbook/assets/image%20%2860%29.png)

g.Enter the **default user name** and **Password**.

![](../../.gitbook/assets/image%20%2863%29.png)



{% hint style="info" %}
**Note**: Get the default user name for the AMI that you used to launch your instance: ‌ 

For a CentOS AMI, the user name is centos. ‌ 

For an Ubuntu AMI, the user name is ubuntu. ‌ 

For a Windows AMI，the user name is administrator.
{% endhint %}

