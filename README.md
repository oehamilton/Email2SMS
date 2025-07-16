# Email2SMS

Custom Lambda to process email and send alarming as simple text to a cell phone
SES writes email to S3 with SNS Notify and Lambda Subscription to SNS
Lambda Reads the S3 Bucket and object from SNS notify and parses the email and attachment for critical alarming information.
Phone number is extracted from the To field.
Customer sends to custom EmailtoSMS domain where SES reads all incoming emails and processes.
