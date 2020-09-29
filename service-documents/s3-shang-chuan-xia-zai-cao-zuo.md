# S3上传/下载操作

一．**Amzon** **S3控台上传下载及CLI命令上传下载到Amazon** **S3**

  在AWS控制台-**服务**搜索S3点击进入（如图5-1），

![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps20.jpg)

图5-1 控制台搜索S3

找到所属S3桶（图5-2），点击进入。![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps21.jpg)

图5-2 找到所属桶

点击上传文件进行上传，添加文件，选择电脑内的一个文件上传，确认要上传的文件上传成功后，会在桶内出现文件，如图5-3所示，也可以创建层级目录文件夹做扩展。

![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps22.jpg)

![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps23.jpg)

![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps24.jpg)

![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps25.jpg)

![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps26.jpg)

图5-3上传文件步骤

注意：当上传文件超过GB时会出现上传过慢或中断的现象，这里推荐一个官方工具

S3 browser: [https://s3browser.com/download/s3browser-9-2-1.exe](https://s3browser.com/download/s3browser-9-2-1.exe) 

  下载文件只需要点击文件，下载按钮完成（url也能下载，如果是未公开桶，需要具有相关AKSK账户的权限才能下载）

![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps27.jpg)

图5-4下载文件步骤

**在linux机器上用CLI下载上传文件：**

在第三步骤我们已经将我们的CLI配置好，现在输入**aws s3 ls**命令，该命令为列出当前账户S3桶。

![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps28.jpg)

图5-5 cli查看S3桶

通过AWS上传命令上传：

**aws s3 cp** **XXXX s3://XXXX/**

![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps29.jpg)

图5-6 S3上传文件

通过AWS下载命令下载：

**aws s3 cp s3://XXXX/XXXX /XXXX/**

![](file:///C:\Users\astra\AppData\Local\Temp\ksohtml2444\wps30.jpg)

参考链接：

控制台：

[https://docs.amazonaws.cn/AmazonS3/latest/user-guide/upload-download-objects.html](https://docs.amazonaws.cn/AmazonS3/latest/user-guide/upload-download-objects.html)

CLI：

[https://docs.aws.amazon.com/cli/latest/reference/s3/](https://docs.aws.amazon.com/cli/latest/reference/s3/)

