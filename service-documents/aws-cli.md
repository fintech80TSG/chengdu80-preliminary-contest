# AWS CLI

## Installing, updating, and uninstalling the AWS CLI <a id="install-cliv2"></a>

This section provides links to information about how to install, update, and uninstall version 2 of the AWS Command Line Interface \(AWS CLI\) on the supported operating systems. 

### Install the AWS CLI version 2 on Linux <a id="cliv2-linux-install"></a>

Follow these steps from the command line to install the AWS CLI on Linux.

We provide the steps in one easy to copy and paste group based on whether you use 64-bit Linux or Linux ARM. See the descriptions of each line in the steps that follow.

**For the latest version of the AWS CLI,** use the following command block:

```text
$ curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

**For a specific version of the AWS CLI,** append a hyphen and the version number to the filename. For this example the filename for version `2.0.30` would be `awscli-exe-linux-x86_64-2.0.30.zip` resulting in the following command:

```text
$ curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64-2.0.30.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

### To install and update for all users using the macOS command line <a id="cliv2-mac-install-cmd-all-users"></a>

If you have `sudo` permissions, you can install the AWS CLI version 2 for all users on the computer.

We provide the steps in one easy to copy and paste group. See the descriptions of each line in the following steps.

**For the latest version of the AWS CLI,** use the following command block:

```text
$ curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
$ sudo installer -pkg AWSCLIV2.pkg -target /
```

**For a specific version of the AWS CLI,** append a hyphen and the version number to the filename. For this example the filename for version `2.0.30` would be `AWSCLIV2-2.0.30.pkg` resulting in the following command:

```text
$ curl "https://awscli.amazonaws.com/AWSCLIV2-2.0.30.pkg" -o "AWSCLIV2.pkg"
$ sudo installer -pkg AWSCLIV2.pkg -target /
```



### Install or update the AWS CLI version 2 on Windows using the MSI installer <a id="cliv2-windows-install"></a>

1. Download the AWS CLI MSI installer for Windows \(64-bit\):

   * **For the latest version of the AWS CLI:** [https://awscli.amazonaws.com/AWSCLIV2.msi](https://awscli.amazonaws.com/AWSCLIV2.msi)
   * **For a specific version of the AWS CLI:** Append a hyphen and the version number to the filename. For this example the filename for version `2.0.30` would be `AWSCLIV2-2.0.30.msi` resulting in the following link [https://awscli.amazonaws.com/AWSCLIV2-2.0.30.msi](https://awscli.amazonaws.com/AWSCLIV2-2.0.30.msi). 

   To update your current installation of AWS CLI version 2 on Windows, download a new installer each time you update to overwrite previous versions. AWS CLI is updated regularly. 

2. Run the downloaded MSI installer and follow the on-screen instructions. By default, the AWS CLI installs to `C:\Program Files\Amazon\AWSCLIV2`.
3. To confirm the installation, open the **Start** menu, search for `cmd` to open a command prompt window, and at the command prompt use the `aws --version` command.

   Don't include the prompt symbol \(`C:\>`\) when you type a command. These are included in program listings to differentiate commands that you type from output returned by the AWS CLI. The rest of this guide uses the generic prompt symbol \(`$`\), except in cases where a command is Windows-specific. 

   ```text
   C:\> aws --version
   aws-cli/2.0.47 Python/3.7.4 Windows/10 botocore/2.0.0
   ```

   If Windows is unable to find the program, you might need to close and reopen the command prompt window to refresh the path, or [add the installation directory to your PATH](https://docs.aws.amazon.com/cli/latest/userguide/install-windows.html#awscli-install-windows-path) environment variable manually.

## Configuring the AWS CLI <a id="cli-chap-configure"></a>

  This section explains how to configure the settings that the AWS Command Line Interface \(AWS CLI\) uses to interact with AWS. These include your security credentials, the default output format, and the default AWS Region.Note

### Quick configuration with aws configure <a id="cli-configure-quickstart-config"></a>

For general use, the aws configure command is the fastest way to set up your AWS CLI installation. When you enter this command, the AWS CLI prompts you for four pieces of information:

```text
$ aws configure
AWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE
AWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
Default region name [None]: us-west-2
Default output format [None]: json
```





\*\*\*\*

