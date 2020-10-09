---
description: Backing up and restoring the computing environment
---

# Backup and Restoring

### Creating a snapshot <a id="ebs-create-snapshot"></a>

Use the following procedure to create a snapshot from the specified volume.

**To create a snapshot using the console**

1. Open the Amazon EC2 console at [https://console.aws.amazon.com/ec2/](https://console.aws.amazon.com/ec2/).
2. Choose **Snapshots** under **Elastic Block Store** in the navigation pane.
3. Choose **Create Snapshot**.
4. For **Select resource type**, choose **Volume**.
5. For **Volume**, select the volume.
6. \(Optional\) Enter a description for the snapshot.
7. \(Optional\) Choose **Add Tag** to add tags to your snapshot. For each tag, provide a tag key and a tag value.
8. Choose **Create Snapshot**.

**To create a snapshot using the command line, see the following example**

* create-snapshot \(AWS CLI\):

```text
aws ec2 create-snapshots \
    --instance-specification InstanceId=i-1234567890abcdef0 \
    --description "This is snapshot of a volume from my-instance"
```

* New-EC2Snapshot \(AWS Tools for Windows PowerShell\):

```text
PS C:\> New-EC2Snapshot -VolumeId vol-12345678 -Description "This is a test"
    
DataEncryptionKeyId :
Description         : This is a test
Encrypted           : False
KmsKeyId            :
OwnerAlias          :
OwnerId             : 123456789012
Progress            :
SnapshotId          : snap-12345678
StartTime           : 12/22/2015 1:28:42 AM
State               : pending
StateMessage        :
Tags                : {}
VolumeId            : vol-12345678
VolumeSize          : 20This example creates a snapshot of the specified volume.
```

### Restoring a snapshot <a id="ebs-create-snapshot"></a>

**To restore a snapshot using the console**

1. Open the Amazon EC2 console at [https://console.aws.amazon.com/ec2/](https://console.aws.amazon.com/ec2/).
2. Choose **Snapshots** in the navigation pane.
3. Select the snapshot and then choose **Actions**, **Create Volume**.
4. Make the snapshot create the Volume with specific AWS accounts as follows:
   * To make the Volume  Same **Availability Zone** as **EC2**.
5. Choose **Save**.
6. Choose broken EC2 and select the root Volume.
7. then choose **Actions, Detach Volume\(Please shut down EC2\)**.
8. Select the new Volume and then choose **Actions,  Attach Volume**.

