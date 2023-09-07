**Detective Controls – Log Maintenance and Retention**

**1. Logs Maintained**

* **Amazon CloudWatch Logs**: We maintain CloudWatch logs to monitor and track the performance metrics and operational health of our applications. This provides us with a centralized view of operational data and actionable insights.

  _Sample Log Entry:_
  ```
  {
     "version":"0",
     "id":"abcd1234",
     "detail-type":"EC2 Instance State-change Notification",
     "source":"aws.ec2",
     "account":"123456789012",
     "time":"yyyy-mm-ddThh:mm:ssZ",
     "region":"us-west-1",
     "resources":[
        "arn:aws:ec2:us-west-1:123456789012:instance/i-1234567890abcdef0"
     ],
     "detail":{
        "instance-id":"i-1234567890abcdef0",
        "state":"running"
     }
  }
  ```

* **VPC Flow Logs**: To capture information about the IP traffic going to and from network interfaces in our VPC, we utilize VPC Flow Logs.

  _Sample Log Entry:_
  ```
  2 123456789010 eni-abc123de 172.31.16.139 172.31.16.21 20641 22 6 20 4249 1418530010 1418530070 ACCEPT OK
  ```

* **ELB Logs**: We utilize Elastic Load Balancer logs to capture detailed information about requests sent to our load balancer.

  _Sample Log Entry:_
  ```
  http 2020-06-10T01:00:00.123456Z my-loadbalancer 192.168.131.39:2817 10.0.0.1:80 0.000086 0.001048 0.001337 200 200 0 57 "GET https://www.example.com:443/ HTTP/1.1" "curl/7.46.0" - -
  ```

* **S3 Bucket Logs**: For auditing access requests to specific buckets, we utilize S3 bucket logging.

  _Sample Log Entry:_
  ```
  a0a1a2a3a4a5a6a7 REQUESTER_PRINCIPAL_ID REST.METHOD[REST_OPERATION] BUCKET_NAME/OBJECT_NAME "REQUEST_URI" REQUESTER_IP HTTP.STATUS s3.ERROR.CODE s3.BYTES_SENT s3.OBJECT_SIZE s3.TOTAL_TIME s3.TURN_AROUND_TIME "referrer" "User-Agent" s3.REQUEST_ID HOST_ID
  ```

* **Application Logs**: Our custom applications have built-in logging to capture critical operations, errors, and user activities.

  _Sample Log Entry:_
  ```
  [2023-09-07 10:10:10] [INFO] User 'john_doe' performed 'LOGIN' action from IP '192.168.1.100'.
  ```

**2. Retention Policy**

All logs are retained as per the customer-agreed retention periods. Our default policy is to retain logs for 90 days. However, for specific customers or projects with specialized requirements, we have extended this period up to 365 days or more, as agreed upon. We utilize Amazon S3 Lifecycle policies to automatically transition logs to the desired storage class or archive/delete them after the defined retention period.

-----------------------


## **Evidence Samples: Detective Controls and Log Maintenance**

**1. AWS CloudWatch Logs**

**Log Sample:**

```
Date: 2023-03-01 Time: 12:32:01
Resource: EC2 Instance (i-0abcd1234efgh5678)
Event: Unauthorized access attempt
Details: Source IP 192.168.0.1 attempted to access without valid credentials

Date: 2023-03-02 Time: 09:15:23
Resource: RDS Database (mydatabase)
Event: Configuration change
Details: Max connections parameter changed from 100 to 150

Date: 2023-03-03 Time: 14:52:45
Resource: Lambda Function (processData)
Event: Invocation Error
Details: Function exceeded maximum execution time

Date: 2023-03-04 Time: 17:34:56
Resource: S3 Bucket (my-data-bucket)
Event: Object deleted
Details: User Admin deleted file data.txt

Date: 2023-03-05 Time: 19:01:12
Resource: DynamoDB Table (userTable)
Event: Scan operation
Details: User ServiceAccount performed a scan operation
```

**Retention Period:** 6 months, as per customer agreement dated 2022-09-01.

---

**2. VPC Flow Logs**

**Log Sample:**

```
Date: 2023-03-01 Time: 11:00:02
Source IP: 10.0.1.12
Destination IP: 10.0.2.15
Action: ACCEPT
Bytes: 1024

Date: 2023-03-01 Time: 11:05:45
Source IP: 10.0.1.12
Destination IP: 13.35.82.129
Action: REJECT
Bytes: 512

Date: 2023-03-01 Time: 11:20:12
Source IP: 10.0.2.15
Destination IP: 13.35.82.129
Action: ACCEPT
Bytes: 2048

Date: 2023-03-01 Time: 12:10:33
Source IP: 10.0.3.18
Destination IP: 10.0.2.15
Action: ACCEPT
Bytes: 1024

Date: 2023-03-01 Time: 12:15:27
Source IP: 10.0.1.12
Destination IP: 13.35.82.130
Action: REJECT
Bytes: 512
```

**Retention Period:** 6 months, as per customer agreement dated 2022-09-01.
