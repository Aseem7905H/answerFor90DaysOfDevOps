# How to Resize EBS Volumes on AWS EC2

In this guide, we’ll walk through how to resize an Elastic Block Store (EBS) volume attached to an EC2 instance. This is useful when your instance runs out of disk space and you need more storage without having to stop and recreate the instance.

## Steps to Resize an EBS Volume:

### 1. Modify the EBS Volume Size

1. **Log into the AWS Console**
   - Go to the [AWS Management Console](https://aws.amazon.com/console/).
   - Navigate to **EC2** under **Services**.
   - In the left-hand navigation pane, under **Elastic Block Store**, click **Volumes**.
   - Select the volume you want to resize.
   - Click **Actions** > **Modify Volume**.
   - Enter the new size in GiB and click **Modify**.

### 2. Extend the Partition on the EC2 Instance

After modifying the volume size, you’ll need to extend the partition within your EC2 instance to utilize the new space.

#### **For Linux Instances:**

1. **Log into the Instance:**
   ```bash
   ssh -i /path/to/your-key.pem ubuntu@<your-instance-public-ip>
   ```

2. **Check Disk Space:**
   ```bash
   df -h
   ```
   This will show your current disk space usage.

3. **Grow the Partition (if necessary):**
   If the volume partition needs to be resized:
   ```bash
   sudo growpart /dev/xvda 1
   ```

4. **Extend the File System:**
   Extend the file system to use the new space.
   ```bash
   sudo resize2fs /dev/xvda1
   ```

5. **Check Disk Space Again:**
   After extending the file system, verify the increased disk space:
   ```bash
   df -h
   ```

### 3. (Optional) Verify Changes in AWS Console
   You can verify the resized volume in the AWS Console by navigating to **Volumes** in the EC2 Dashboard and checking the new size.

## Conclusion
Resizing an EBS volume is a straightforward process that involves modifying the volume size in AWS and then extending the file system within the instance. This allows you to easily scale your storage without downtime or the need to recreate the instance.

