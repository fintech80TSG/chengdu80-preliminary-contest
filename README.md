# CHENGDU80  ONLINE MANUAL

## Intro

CHENGDU80 is a FinTech design and development competition for academic participants utilizing open source technology. As part of the SWUFE-CDAR annual conference, the Chengdu 80 competition will provide opportunities for students to interact with leading academics in finance and technology, international financial institutions, and government and regulatory leaders. Each participating team will consist of up to 6 students from a single academic institution led by a faculty member or postdoctoral scholar and must include members of both genders and at least 1 undergraduate.

This document site is an introduction to the technical rules and environment of the CHENGDU80 contest. Participants should be informed of the environment, technical process and service request means described in this document in advance.

The guide of this contest is as follows. Please read it carefully:

### 1. **Join the CHENGDU80 @MICROSOFT TEAMS** <a id="user-sign-in-page"></a>

    **** [Download](https://www.microsoft.com/en/microsoft-365/microsoft-teams/download-app#desktopAppDownloadregion) Teams APP --&gt; [Regist](https://support.microsoft.com/en-us/office/sign-up-for-teams-free-70aaf044-b872-4c32-ac47-362ab29ebbb1?ui=en-us&rs=en-us&ad=us)  Account --&gt; [Join](%20https://teams.microsoft.com/l/team/19%3ab5064e81a1f74d82bc1f6fc909bcf86a%40thread.tacv2/conversations?groupId=b6ecae3d-b84a-4648-acc2-73b4e8c3369e&tenantId=64e0c74b-1a17-4000-81c9-28cc776f6c75) CHENGDU80

### **2**. **Complete the Information** <a id="user-sign-in-page"></a>

      Complete info [Form](https://forms.office.com/Pages/ResponsePage.aspx?id=S8fgZBcaAECBySjMd29sdbARWGwIoxVBvYOnmX6MKMNUM1pHRU9KSTVBNVBIUUlYNkRCVk5YUFBNRC4u) ,includs : the nearest Region, OS,  **test appointment,** Account Email.  
      The test time range is CST 2020-10-22 00:00 to CST 2020-10-23:00 

### 3.  **Test  Environment**

       At the appointment time at step 2 , Follow the checklist below：

      **Test Operation**:  

                      Target 1-[EC2 login is available](operation-manual/environment-test.md#3-1-test-connection-to-ec2),

                      Target 2-[Test Conneion](operation-manual/environment-test.md#3-2-test-ec2-connection-speed)[ Speed](operation-manual/environment-test.md#3-2-test-ec2-connection-speed),

                      Target 3-[S3 upload/download test](operation-manual/environment-test.md#3-3-test-s3-upload-download).

       **Feedback**: After the TEST, please feedback your result via this [form](https://forms.office.com/Pages/ResponsePage.aspx?id=S8fgZBcaAECBySjMd29sdbARWGwIoxVBvYOnmX6MKMNUQUIwNEQ3SDE2UDJDOEE5MThEVllLTFpRUC4u).

###   4.  **Upload the Video of Team Intro**  <a id="user-sign-in-page"></a>

       **** The [operation guide](operation-manual/upload-team-introduction-video.md) for uploading to S3

###    **5**. During **The Competition**  <a id="user-sign-in-page"></a>

        **Starting Time：** CST 2020-10-26 14:00 to CST 2020-10-29 22:00

Operation manual:

5.1  [Connect to EC2](operation-manual/competition-operation/connect-to-ec2.md)

5.2  [Backup and Restore](operation-manual/competition-operation/backup-and-restore.md)

5.3  [Obtaining Data](operation-manual/competition-operation/obtaining-data.md)

5.4  [Code Submission](operation-manual/competition-operation/code-submission.md)

5.5  [Prototype Deployment](operation-manual/competition-operation/prototype-deployment.md)

5.6  [Video Upload](operation-manual/competition-operation/upload-team-introduction-video.md)

###      **6**. **The End of the Contest** <a id="user-sign-in-page"></a>

6.1 By the end of the contest ,CST 2020-10-29 22:00 , all servers will be fully backed up and copies are downloaded for review.;

6.2 All teams need to **shut down** your servers and also ensure that your servers provide access to the deployed prototypes without any configuration once they are up again.

###     **7**. Submit Presentation Videos <a id="user-sign-in-page"></a>

Each team can access the services provided by its own server between CST **2020-10-30 08:00- 2020-10-31 08:00**, whether it is a B/S or C/S architecture. But cannot log into the server to make code changes. When the service does not start properly, a login can be requested within TEAMS and all actions will be logged. 

The deadline for [uploading the video](operation-manual/competition-operation/upload-team-introduction-video.md) is CST 2020-10-31 08:00.

###     **8**. **Technical Support on Duty** <a id="user-sign-in-page"></a>

All technical support services will be available on the Teams platform. Please ask your questions on the Teams platform and @ support@chengdu80.org or Help@chengdu80.org or admin@chengdu80.org

{% hint style="info" %}
The document will be updated according to the rules of the contest announced by the Committee. Relevant technical explanations and rule interpretations shall be subject to the official interpretation of the chengdu80 contest committee.
{% endhint %}



