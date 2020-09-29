# 配置

**Configuration of EC2**

### `1. Launch an instance` <a id="ec2-launch-instance"></a>

1. Open the Amazon EC2 console at [https://console.aws.amazon.com/ec2/](https://console.aws.amazon.com/ec2/).
2. From the console dashboard, choose **Launch Instance**.
3. The **Choose an Amazon Machine Image \(AMI\)** page displays a list of basic configurations, called _Amazon Machine Images \(AMIs\)_, that serve as templates for your instance. Select an HVM version of Amazon Linux 2. Notice that these AMIs are marked "Free tier eligible."
4. On the **Choose an Instance Type** page, you can select the hardware configuration of your instance. Select the `t2.micro` instance type, which is selected by default. The `t2.micro` instance type is eligible for the free tier. In Regions where `t2.micro` is unavailable, you can use a `t3.micro` instance under the free tier. 
5. Choose **Review and Launch** to let the wizard complete the other configuration settings for you.
6. On the **Review Instance Launch** page, under **Security Groups**, you'll see that the wizard created and selected a security group for you. You can use this security group, or alternatively you can select the security group that you created when getting set up using the following steps:
   1. Choose **Edit security groups**.
   2. On the **Configure Security Group** page, ensure that **Select an existing security group** is selected.
   3. Select your security group from the list of existing security groups, and then choose **Review and Launch**.
7. On the **Review Instance Launch** page, choose **Launch**.
8. When prompted for a key pair, select **Choose an existing key pair**, then select the key pair that you created when getting set up.Warning

   Don't select **Proceed without a key pair**. If you launch your instance without a key pair, then you can't connect to it.

   When you are ready, select the acknowledgement check box, and then choose **Launch Instances**.

9. A confirmation page lets you know that your instance is launching. Choose **View Instances** to close the confirmation page and return to the console.
10. On the **Instances** screen, you can view the status of the launch. It takes a short time for an instance to launch. When you launch an instance, its initial state is `pending`. After the instance starts, its state changes to `running` and it receives a public DNS name. \(If the **Public DNS \(IPv4\)** column is hidden, choose **Show/Hide Columns** \(the gear-shaped icon\) in the top right corner of the page and then select **Public DNS \(IPv4\)**.\)
11. It can take a few minutes for the instance to be ready so that you can connect to it. Check that your instance has passed its status checks; you can view this information in the **Status Checks** column.



**`2. To terminate your instance`**

1. In the navigation pane, choose **Instances**. In the list of instances, select the instance.
2. Choose **Actions**, **Instance State**, **Terminate**.
3. Choose **Yes, Terminate** when prompted for confirmation.

   Amazon EC2 shuts down and terminates your instance. After your instance is terminated, it remains visible on the console for a short while, and then the entry is deleted.

