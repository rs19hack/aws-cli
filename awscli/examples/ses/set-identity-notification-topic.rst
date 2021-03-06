**To set the Amazon SNS topic to which Amazon SES will publish bounce and complaint notifications for a verified identity**

The following example uses the ``set-identity-notification-topic`` command to specify the Amazon SNS topic to which a verified email address will receive bounce notifications::

    aws ses set-identity-notification-topic --identity user@example.com --notification-type Bounce --sns-topic arn:aws:sns:us-east-1:EXAMPLE65304:MyTopic

Output::    

 {
    "ResponseMetadata": {
        "RequestId": "f09187e2-d48e-11e2-9349-ff3ea16d1ca0"
    }
 }

For more information about feedback notifications, see `Bounce and Complaint Notifications in Amazon SES`_ in the *Amazon Simple Email Service Developer Guide*.

.. _Bounce and Complaint Notifications in Amazon SES: http://docs.aws.amazon.com/ses/latest/DeveloperGuide/bounce-complaint-notifications.html

