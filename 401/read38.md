# [SNS: Getting Started](https://aws.amazon.com/sns/getting-started/)

### To get start with Simple Notification Service (SNS) :
1. **Create a topic** -> by visiting [Amazon SNS console](https://console.aws.amazon.com/sns/v3/home) you can create a topic.
2. **Create a subscription to the topic**
3. **Publish a message to the topic** 
4. **Delete the subscription and topic**


# [SNS with Amplify (and Firebase)](https://docs.amplify.aws/)

### Usage of SNS(adding Push Notifications into their mobile app) with amplify:

1. **Asynchronous actions**, such as when an order is placed through an app, and confirmation or status notifications are sent to the user.
2. **Scheduled reminders**
3. **Instant messaging**, where your app provides two-way communication (i.e., chat).


# Notifications

To create your Android platform application in Amazon SNS, you must have credentials from Firebase Cloud Messaging (FCM).

### Create a Firebase project on the Firebase website:

1. In the Firebase console, choose your project.

2. In the left navigation pane, choose the gear icon, and then choose Project settings.

3. Choose Cloud Messaging.

4. Under Project credentials, find the Server key. This your FCM project's API key. Copy it to your clipboard.

### Create a platform application in Amazon SNS

1.  Open the Amazon SNS console.

2.  In the left navigation pane, choose Mobile. Then, choose Push notifications.

3.  On the Mobile push notifications page, next to Platform applications, choose Create platform application.

4.  On the Create platform application page, under Details, do the following:
    For Application name, enter the name of your application.
    For Push notification platform, choose Firebase Cloud Messaging (FCM).
    Under Firebase Cloud Messaging Credentials, for API key, enter the server key that you copied earlier.

5.  (Optional) Set up event notifications and delivery status logging.

6.  Choose Create platform application.