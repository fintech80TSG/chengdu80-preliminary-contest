# 账户登录



Welcome to the [AWS Management Console](https://console.aws.amazon.com/). This guide provides a short introduction to working with the console. To learn how to work with individual services in the console, see [AWS Documentation](https://aws.amazon.com//documentation/).

**Topics**

* [What is the AWS Management Console?](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html#learn-whats-new)
* [Getting started with a service](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html#start-service)
* [Adding and removing favorites](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html#add-remove-shortcut)
* [Choosing a Region](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html#select-region)
* [Changing your password](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html#change-password)
* [Getting billing information](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html#get-billinginfo)
* [Using the device of your choice](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html#console-device)
* [Troubleshooting](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html#troubleshooting)

### What is the AWS Management Console? <a id="learn-whats-new"></a>

The [AWS Management Console](https://console.aws.amazon.com/) is a web application that comprises and refers to a broad collection of service consoles for managing Amazon Web Services. When you first sign in, you see the console home page.

![](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/images/console-home.png)

The home page provides access to each service console as well as an intuitive user interface for exploring AWS and getting helpful tips. Among other things, the individual service consoles offer tools for working with [Amazon S3](https://console.aws.amazon.com/s3/) buckets, launching and connecting to [Amazon EC2](https://console.aws.amazon.com/ec2/) instances, setting [Amazon CloudWatch](https://console.aws.amazon.com/cloudwatch/) alarms, and getting information about your account and about [billing](https://console.aws.amazon.com/billing/).

![](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/images/console-parts-new.png)



### Getting started with a service <a id="start-service"></a>

The [AWS Management Console](https://console.aws.amazon.com/) provides multiple ways for navigating to individual service consoles.

**To open a console for a service**

Do one of the following:

* In the **Find Services** box, enter the name of the service. Then choose the service that you want from the list of search results.
* Under **Recently visited services**, choose a service name.
* Under **All services**, choose a service name.
* On the navigation bar, choose **Services** to open a full list of services. Then choose the service that you want.

![                                  ](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/images/console-search.png)

### Adding and removing favorites <a id="add-remove-shortcut"></a>

For easy access, you can save the consoles that you use the most to a list of **Favorites**.

**To add a service to the list of Favorites**

1. On the navigation bar, choose **Services**.
2. In either the **Recently visited** list or the **All services** list, pause on the name of the service that you want to add as a favorite.
3. Select the star to the left of the service name.
4. Repeat the previous two steps to add more services to your **Favorites** list.

![                        The Services menu shows favorites, recently visited, and all                            services                    ](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/images/console-favorite.png)

**To remove a service from the list of Favorites**

1. On the navigation bar, choose **Services**.
2. Do one of the following:
   * In the **Favorites** list, pause on the name of a service. Then choose the **X** to the right of the service name.
   * In the **Recently visited** list or **All services** list, deselect the star by the name of a service that is in your **Favorites** list.

### Choosing a Region <a id="select-region"></a>

For many services, you can choose an AWS Region that specifies where your resources are managed. You do not choose a Region for the [AWS Management Console](https://console.aws.amazon.com/) or for some services, such as IAM.

**To choose a Region**

1. In the AWS Management Console, [choose a service](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html#start-service) to go to that service's console.
2. On the navigation bar, choose the name of the currently displayed Region. Then choose the Region you want to change to.

   When you choose a Region, that Region becomes the default in the console.

![                                       ](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/images/console-region-selector.png)

### Changing your password <a id="change-password"></a>

If you are an account owner, you can change your AWS account password from the [AWS Management Console](https://console.aws.amazon.com/).

**To change your password**

1. On the navigation bar, choose your account name.
2. Choose **My Security Credentials**.
3. The page that you see varies with the type of account that you used to sign in. Follow the console instructions to get to the page for changing your password.
4. Enter your current password once and your new password twice.

   The new password must be at least eight characters long and must include a symbol, a number, an uppercase letter, and a lowercase letter.

5. When you've completed the password form, choose **Change Password** or **Save changes**.

### Getting billing information <a id="get-billinginfo"></a>

If you have the necessary permissions, you can get information about your AWS charges from the console.

**To get your billing information**

1. On the navigation bar, choose your account name.
2. Choose **My Billing Dashboard**.
3. Use the AWS Billing and Cost Management dashboard to find a summary and a breakdown of your monthly spending. To learn more, see the [AWS Billing and Cost Management User Guide](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/).

### Using the device of your choice <a id="console-device"></a>

The [AWS Management Console](https://console.aws.amazon.com/) has been designed to work on tablets as well as other kinds of devices:

* Horizontal and vertical space is maximized to show more on your screen.
* Buttons and selectors are larger for a better touch experience.

The AWS Management Console is also available as an app for Android and iOS. This app provides mobile-relevant tasks that are a good companion to the full web experience. For example, you can easily view and manage your existing Amazon EC2 instances and Amazon CloudWatch alarms from your phone.

You can download the AWS Console mobile app from [Amazon Appstore](http://www.amazon.com/AWS-Mobile-LLC-Console/dp/B00ATSN730), [Google Play](https://play.google.com/store/apps/details?id=com.amazon.aws.console.mobile), or [iTunes](https://itunes.apple.com/us/app/aws-console/id580990573?mt=8).

### Troubleshooting <a id="troubleshooting"></a>

Consult this section to find solutions to common problems with the AWS Management Console.

#### Fix page load issues with Internet Explorer 11 <a id="ie11"></a>

If you use the [AWS Management Console](https://console.aws.amazon.com/) with Internet Explorer 11, the browser might fail to load some pages of the console. This is a problem related to Internet Explorer's Compatibility View. To address this issue, in Internet Explorer, open **Compatibility View Settings** and disable **Display intranet sites in Compatibility View**.

For more information, see [Fix site display problems with Compatibility View](https://support.microsoft.com/en-us/help/17472/windows-internet-explorer-11-fix-site-display-problems-compatibility-v#ie=ie-11).

