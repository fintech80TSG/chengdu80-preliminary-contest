# Access to Account

### Sign in as an IAM user <a id="user-sign-in-page"></a>

1.Open a browser and enter the following sign-in URL, replacing `account_alias_or_id` with the account alias or account ID provided by your administrator.

```text
https://account_alias_or_id.signin.aws.amazon.com/console/
```

2.Enter your IAM user name and password and choose **Sign in**.

                                ![
            IAM User Sign-in Page
          ](https://docs.aws.amazon.com/IAM/latest/UserGuide/images/sign-in-iam-user-capture.png)

### Check in EC2 <a id="user-sign-in-page"></a>

1.select **Services -&gt; EC2** buttons

![](../.gitbook/assets/image%20%2857%29.png)

2.get EC2 information



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

**To connect to your instance using SSH**

1. In a terminal window, use the **ssh** command to connect to the instance. You specify the path and file name of the private key \(`.pem`\), the user name for your instance, and the public DNS name or IPv6 address for your instance

   * \(Public DNS\) To connect using your instance's public DNS name, enter the following command.

     ```text
     ssh -i /path/my-key-pair.pem my-instance-user-name@my-instance-public-dns-name
     ```

   * \(IPv6\) Alternatively, if your instance has an IPv6 address, to connect using your instance's IPv6 address, enter the following command.

     ```text
     ssh -i /path/my-key-pair.pem my-instance-user-name@my-instance-IPv6-address
     ```

   You see a response like the following:

   ```text
   The authenticity of host 'ec2-198-51-100-1.compute-1.amazonaws.com (198-51-100-1)' can't be established.
   ECDSA key fingerprint is l4UB/neBad9tvkgJf1QZWxheQmR59WgrgzEimCG6kZY.
   Are you sure you want to continue connecting (yes/no)?
   ```

2. \(Optional\) Verify that the fingerprint in the security alert matches the fingerprint that you previously obtained in [\(Optional\) Get the instance fingerprint](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/connection-prereqs.html#connection-prereqs-fingerprint). 
3. Enter `yes`.

   You see a response like the following:

   ```text
   Warning: Permanently added 'ec2-198-51-100-1.compute-1.amazonaws.com' (ECDSA) to the list of known hosts.
   ```

**Connect using PuTTY** 

\*\*\*\*

**windows 2016 R2**

use

