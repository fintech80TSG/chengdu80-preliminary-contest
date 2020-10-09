# Access to Account

### Sign in as an IAM user <a id="user-sign-in-page"></a>

Before you sign into an AWS account as an IAM user, be sure that you have the following required information. If you do not have this information, contact the administrator for the AWS account.

**Requirements**

* One of the following:
  * The account alias.
  * The 12-digit AWS account ID.
* The user name for your IAM user.
* The password for your IAM user.

If you are an IAM user, you can log in using either a sign-in URL or the main sign-in page.

**To sign in to an AWS account as an IAM user using an IAM users sign-in URL**

1. Open a browser and enter the following sign-in URL, replacing `account_alias_or_id` with the account alias or account ID provided by your administrator.

   ```text
   https://account_alias_or_id.signin.aws.amazon.com/console/
   ```

2. Enter your IAM user name and password and choose **Sign in**.

                                ![
            IAM User Sign-in Page
          ](https://docs.aws.amazon.com/IAM/latest/UserGuide/images/sign-in-iam-user-capture.png)

**To sign in to an AWS account as an IAM user using the main sign-in page**

1. Open [https://console.aws.amazon.com/](https://console.aws.amazon.com/).
2. If you have not signed in previously using this browser, the main sign-in page appears. Choose **IAM user**, enter the account alias or account ID, and choose **Next**.

                               ![
            Main sign-in page with IAM user selected
          ](https://docs.aws.amazon.com/IAM/latest/UserGuide/images/sign-in-main-capture-iam.png)

If you have signed in as an IAM user previously using this browser, your browser might remember the account alias or account ID for the AWS account. If so, you'll see the screen shown in the next step instead.

1. Enter your IAM user name and password and choose **Sign in**.

                               ![
            IAM User Sign-in Page
          ](https://docs.aws.amazon.com/IAM/latest/UserGuide/images/sign-in-iam-user-capture.png)

If you have signed in as an IAM user for a different AWS account previously using this browser, or you need to sign in as a root user instead, choose **Sign in using root user email** to return to the main sign-in page.

