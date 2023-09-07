
## **Evidence: Detective Controls and Log Maintenance**

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

---

This is just a fictional representation for illustration purposes. In reality, you would extract real logs from your AWS management console, ensuring all sensitive or identifying data is redacted. Make sure to also have proper documentation to support your retention periods like customer agreements or policies.