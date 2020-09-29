# S3上传/下载操作

一．**Amzon** **S3控台上传下载及CLI命令上传下载到Amazon** **S3**

  在AWS控制台-**服务**搜索S3点击进入（如图5-1），

![&#x56FE;5-1 &#x63A7;&#x5236;&#x53F0;&#x641C;&#x7D22;S3](../.gitbook/assets/image%20%2848%29.png)

找到所属S3桶（图5-2），点击进入。![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps21.jpg)

![&#x56FE;5-2 &#x627E;&#x5230;&#x6240;&#x5C5E;&#x6876;](../.gitbook/assets/image%20%2847%29.png)

点击上传文件进行上传，添加文件，选择电脑内的一个文件上传，确认要上传的文件上传成功后，会在桶内出现文件，如图5-3所示，也可以创建层级目录文件夹做扩展。

![](../.gitbook/assets/image%20%2837%29.png)

![](../.gitbook/assets/image%20%2840%29.png)

![](../.gitbook/assets/image%20%2838%29.png)

![](../.gitbook/assets/image%20%2843%29.png)

![&#x56FE;5-3&#x4E0A;&#x4F20;&#x6587;&#x4EF6;&#x6B65;&#x9AA4;](../.gitbook/assets/image%20%2839%29.png)



注意：当上传文件超过GB时会出现上传过慢或中断的现象，这里推荐一个官方工具

S3 browser: [https://s3browser.com/download/s3browser-9-2-1.exe](https://s3browser.com/download/s3browser-9-2-1.exe) 

  下载文件只需要点击文件，下载按钮完成（url也能下载，如果是未公开桶，需要具有相关AKSK账户的权限才能下载）

![&#x56FE;5-4&#x4E0B;&#x8F7D;&#x6587;&#x4EF6;&#x6B65;&#x9AA4;](../.gitbook/assets/image%20%2844%29.png)

图5-4下载文件步骤

**在linux机器上用CLI下载上传文件：**

在第三步骤我们已经将我们的CLI配置好，现在输入**aws s3 ls**命令，该命令为列出当前账户S3桶。

![&#x56FE;5-5 cli&#x67E5;&#x770B;S3&#x6876;](../.gitbook/assets/image%20%2851%29.png)

 

通过AWS上传命令上传：

**aws s3 cp** **XXXX s3://XXXX/**

![&#x56FE;5-6 S3&#x4E0A;&#x4F20;&#x6587;&#x4EF6;](../.gitbook/assets/image%20%2841%29.png)

图5-6 S3上传文件

通过AWS下载命令下载：

**aws s3 cp s3://XXXX/XXXX /XXXX/**

![ ](../.gitbook/assets/image%20%2850%29.png)

参考链接：

控制台：

[https://docs.amazonaws.cn/AmazonS3/latest/user-guide/upload-download-objects.html](https://docs.amazonaws.cn/AmazonS3/latest/user-guide/upload-download-objects.html)

CLI：

[https://docs.aws.amazon.com/cli/latest/reference/s3/](https://docs.aws.amazon.com/cli/latest/reference/s3/)

