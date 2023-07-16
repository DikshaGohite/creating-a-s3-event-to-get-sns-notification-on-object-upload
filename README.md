Project Description: Creating an S3 event to receive a email notification for a object upload event with SNS 

Services used: Amazon S3, Amazon SNS

Section 1: Creating a S3 Bucket

1. Navigate to the Amazon S3 service by typing "S3" in the AWS service search bar and selecting the Amazon S3 option that appears.
2. In the Amazon S3 dashboard, click the "Create bucket" button. A dialog box will appear.
3. Provide Bucket Name: Enter a unique and meaningful name for your bucket. Bucket names must be globally unique across all AWS accounts
4. Keep other settings as default, scroll to the bottom of the page and select create bucket.

![](1.JPG)

Section 2: Creating a SNS topic and Subscription

1. In the AWS Management Console search bar and select the "Simple Notification Service" option from the results.
2. In the SNS dashboard, click on the "Create topic" button to start creating a new SNS topic.
3. Select Standard topic, assign a name to your topic then scroll to the bottom of your page and click create topic

Your configuration will look something like this:
![](2.PNG)
![](3.PNG)

4. Now we have to create a subscription for this SNS topic so that we can receive notifications published to the topic
5. In the above screenshot you will see a create "subscription button" select that
6. In the new window select the Topic ARN (ARN of your SNS topic), protocol and Endpoint as below and hit the "Create Subscription" button at the bottom of the Page
![](4.PNG)

7. The last thing now left to do is confirming the subscription, check your email from Amazon and confirm subscription
![](5.PNG)

Scetion 3: Creating a S3 event notification

