# Access to Account

### Sign in as an IAM user <a id="user-sign-in-page"></a>

1.You will get the `account_alias_or_id` and `password` from the email.

2.Open a browser and enter the following sign-in URL, replacing `account_alias_or_id` with the account alias or account ID provided by your administrator.

```text
https://account_alias_or_id.signin.aws.amazon.com/console/
```

3.Enter your IAM user name and password and choose **Sign in**.

                                ![
            IAM User Sign-in Page
          ](https://docs.aws.amazon.com/IAM/latest/UserGuide/images/sign-in-iam-user-capture.png)

### Check in EC2 <a id="user-sign-in-page"></a>

1.select **Services -&gt; EC2** buttons

![](../.gitbook/assets/image%20%2864%29.png)

2.get EC2 information

Port groups are restricted in this competition. The range of port groups is XXX-XXX.

![](../.gitbook/assets/image%20%2862%29.png)

### Sign in EC2 <a id="user-sign-in-page"></a>

**Get the default user name for the AMI that you used to launch your instance:**

 For a CentOS AMI, the user name is `centos`. ****

 For an Ubuntu AMI, the user name is `ubuntu`.

 For a Windows AMI，the user name is `administrator`.

**centos7 or ubuntu18.04 LTS**

**Connect using SSH**

1.Install an SSH client on your local computer as needed

Your local computer might have an SSH client installed by default. You can verify this by typing **ssh** at the command line. If your compute doesn't recognize the command, you can install an SSH client.

* Recent versions of Windows Server 2019 and Windows 10 - OpenSSH is included as an installable component. For information, see [OpenSSH in Windows](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_overview).
* Earlier versions of Windows - Download and install OpenSSH. For more information, see [Win32-OpenSSH](https://github.com/PowerShell/Win32-OpenSSH/wiki).
* Linux and macOS X - Download and install OpenSSH. For more information, see [http://www.openssh.com](http://www.openssh.com/).

2. Connect your Linux instance using an SSH client

Use the following procedure to connect to your Linux instance using an SSH client. 

1. In a terminal window, use the **ssh** command to connect to the instance. You specify the path and file name of the private key \(`.pem`\), the user name for your instance, and the public DNS name or IPv6 address for your instance

{% tabs %}
{% tab title="Public DNS" %}
\(Public DNS\) To connect using your instance's public DNS name, enter the following command.

```text
ssh -i /path/my-key-pair.pem my-instance-user-name@my-instance-public-dns-name
```
{% endtab %}

{% tab title="IPv6" %}
\(IPv6\) Alternatively, if your instance has an IPv6 address, to connect using your instance's IPv6 address, enter the following command.

```
ssh -i /path/my-key-pair.pem my-instance-user-name@my-instance-IPv6-address
```
{% endtab %}
{% endtabs %}

You see a response like the following:

```text
The authenticity of host 'ec2-198-51-100-1.compute-1.amazonaws.com (198-51-100-1)' can't be established.
ECDSA key fingerprint is l4UB/neBad9tvkgJf1QZWxheQmR59WgrgzEimCG6kZY.
Are you sure you want to continue connecting (yes/no)?
```

Enter `yes`.

You see a response like the following:

```text
Warning: Permanently added 'ec2-198-51-100-1.compute-1.amazonaws.com' (ECDSA) to the list of known hosts.
```

**Connect using PuTTY** 

1.  Download and install PuTTY from the [PuTTY download page](http://www.chiark.greenend.org.uk/~sgtatham/putty/). 
2. Start PuTTY \(from the **Start** menu, choose **All Programs, PuTTY, PuTTY**\).
3. In the **Category** pane, choose **Session** and complete the following fields:

   1. In the **Host Name** box, do one of the following:

   * \(Public DNS\) To connect using your instance's public DNS name, enter `my-instance-user-name`@`my-instance-public-dns-name`.
   * \(IPv6\) To connect using your instance's IPv6 address, enter  `my-instance-user-name`@`my-instance-IPv6-address`.

   1. Ensure that the **Port** value is 22.
   2. Under **Connection type**, select **SSH**.

                               ![
   							PuTTY configuration - Session
   						](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/images/putty-session-config.png)



{% hint style="info" %}
 \(Optional\) You can configure PuTTY to automatically send 'keepalive' data at regular intervals to keep the session active. This is useful to avoid disconnecting from your instance due to session inactivity. In the **Category** pane, choose **Connection**, and then enter the required interval in the **Seconds between keepalives** field. For example, if your session disconnects after 10 minutes of inactivity, enter 180 to configure PuTTY to send keepalive data every 3 minutes.
{% endhint %}

1. In the **Category** pane, expand **Connection**, expand **SSH**, and then choose **Auth**. Complete the following:

   1. Choose **Browse**.
   2. Select the `.ppk` file that you generated for your key pair and choose **Open**.
   3. \(Optional\) If you plan to start this session again later, you can save the session information for future use. Under **Category**, choose **Session**, enter a name for the session in **Saved Sessions**, and then choose **Save**.
   4. Choose **Open**.

   Other SSH client please find the information about SSH Client.

**windows 2016 R2**

1. Open the Amazon EC2 console at [https://console.aws.amazon.com/ec2/](https://console.aws.amazon.com/ec2/).
2. Choose **EC2** enter the Page.
3. Choose **Connect**. 

![](../.gitbook/assets/image%20%2861%29.png)

1. Select the file name of the private key \(`.pem`\) and unzip.
2. Copy **EC2 Password**.
3. Using Windows mstsc\(Remote Desktop Connection\) to connect.

![](../.gitbook/assets/image%20%2860%29.png)

1. Enter the **default user name** and **Password**.

![](../.gitbook/assets/image%20%2863%29.png)

