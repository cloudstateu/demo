 <img src="/img/logo.png" alt="Chmurowisko logo" width="200" align="right">
  <br><br>
  <br><br>
  <br><br>

# Creating Amazon EC2 Instances (for Linux)

## LAB Overview

#### This lab leads you through the steps to launch and configure your first virtual machine in the Amazon cloud. You will learn about using Amazon Machine Images to launch Amazon EC2 instances, creating key pairs for SSH authentication, securing network access to Amazon EC2 instances with security groups.

## Task 1: Launch a Linux instance

1. On the **Services** menu, click **EC2**.
2. Click **Launch Instance**.
3. On the left panel select **My AMIs**.
4. Below in the section **Overnship** make sure **Shared with me** is selected.
5. Select **WebsiteTST** AMI.
6. On the **Choose an Instance Type** page, select the **t2.micro** instance type, which should be automatically selected.
7. Click **Next: Configure Instance Details**.
8. On the **Configure Instance Details** page provide the following information:
   * **Number of instance**: 1
   * **Network:** Leave the DefaultVPC
   * **Auto-assign Public IP**: Enable
9. Click **Next: Add Storage**. 
10. Click **Next: Add Tags** to accept the default storage device configuration.
11. On the **Add Tags** page, click **Add Tag,** type a **Name** for a Key box and YOUR_NAME in the Value box.
12. Click **Next: Configure Security Group**.
13. For **Assign a security group**, select **select an existing security group** and select a **Lukasz** Security Group.
14. Click **Review and Launch**. 

**Note:** You may see a warning on this screen that **Your security group is open to the world**. This is a result of not restricting SSH access to your machine, as described above. For the purposes of this lab only, you may ignore this warning.

15. Review your choices, and then click **Launch**.
16. In the key pair dialog box, select **Proceed without a key pair**.
17. Select "I acknowladge....".
18. Click **Launch Instances**.
19. On the status page, which notifies you that your instances are launching, click **View Instances**.


## Task 2: Connect to your EC2 instance.

20. On the list select your EC2 instance.
21. Below in the **Description** tab, look for **Public DNS (IPv4)**.
22. Copy the value of **Public DNS (IPv4)**.
23. Open the new web brower window.
24. Paste the URL and hit enter.
25. You application **Hello World** should appear.

![helloworld](/img/helloworld.png)

## END LAB

This is the end of the lab.

<center><p>&copy; 2019 Chmurowisko Sp. z o.o.<p></center>
