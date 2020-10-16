# Connect to EC2

**Get the default user name for the AMI that you used to launch your instance:**

 For a CentOS AMI, the user name is `centos`. ****

 For an Ubuntu AMI, the user name is `ubuntu`.

 For a Windows AMI，the user name is `administrator`.

**centos7 or ubuntu18.04 LTS**

**Connect using PuTTY** 

a. Download and install PuTTY from the [PuTTY download page](http://www.chiark.greenend.org.uk/~sgtatham/putty/). 

b.Start PuTTY \(from the **Start** menu, choose **All Programs, PuTTY, PuTTY**\).

c.In the **Category** pane, choose **Session** and complete the following fields:

1. In the **Host Name** box, do one of the following:

* \(Public DNS\) To connect using your instance's public DNS name, enter `my-instance-user-name`@`my-instance-public-dns-name`.
* \(IPv6\) To connect using your instance's IPv6 address, enter  `my-instance-user-name`@`my-instance-IPv6-address`.

d.Ensure that the **Port** value is 22.

f.Under **Connection type**, select **SSH**.

                            ![
							PuTTY configuration - Session
						](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/images/putty-session-config.png)



{% hint style="info" %}
 \(Optional\) You can configure PuTTY to automatically send 'keepalive' data at regular intervals to keep the session active. This is useful to avoid disconnecting from your instance due to session inactivity. In the **Category** pane, choose **Connection**, and then enter the required interval in the **Seconds between keepalives** field. For example, if your session disconnects after 10 minutes of inactivity, enter 180 to configure PuTTY to send keepalive data every 3 minutes.
{% endhint %}

g.In the **Category** pane, expand **Connection**, expand **SSH**, and then choose **Auth**. Complete the following:

1. Choose **Browse**.
2. Select the `.ppk` file that you generated for your key pair and choose **Open**.
3. \(Optional\) If you plan to start this session again later, you can save the session information for future use. Under **Category**, choose **Session**, enter a name for the session in **Saved Sessions**, and then choose **Save**.
4. Choose **Open**.

Other SSH client please find the information about [SSH Client](https://www.slant.co/topics/149/~best-ssh-clients-for-windows).

**windows 2016 R2**

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

