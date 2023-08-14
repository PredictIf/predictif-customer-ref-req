# Security Engagement Standard Operating Procedures (SOPs)
## AWS Account Creation on Behalf of Customers

### Purpose:
To ensure the secure creation and management of AWS accounts on behalf of customers, while maintaining the highest standards of security and compliance.

### Scope:
This SOP applies to all personnel involved in the creation and management of AWS accounts for customers.

### Procedure:

1. **AWS Account Creation**:
    - Always use the AWS Organizations feature to create new accounts. This ensures that the accounts are under the control of the main organization and can benefit from centralized policies and controls.
    - Ensure that the account name, alias, and other identifiers are consistent with the naming conventions established by the organization.

2. **Usage of Root Account**:
    - The root account should **never** be used for day-to-day workload activities. It should only be used for initial setup and certain administrative tasks that can't be performed by IAM users or roles.
    - After initial setup, the root account credentials should be securely stored, preferably in a hardware security module (HSM) or a secure vault, and accessed only under exceptional circumstances.

3. **Enable Multi-Factor Authentication (MFA) on Root**:
    - Immediately after account creation, enable MFA on the root account.
    - Use a hardware MFA device or a virtual MFA on a secure device.
    - Store the MFA backup codes in a secure location, separate from the root account credentials.

4. **Setting Contact Information**:
    - Set the contact email address to a corporate email address. This ensures that any notifications or alerts related to the account are sent to the organization and not to an individual.
    - If a phone number is required, use a corporate phone number.

5. **Enable CloudTrail Logs**:
    - Enable AWS CloudTrail in all regions, ensuring that all activities across the account are logged.
    - Create a new S3 bucket dedicated to storing CloudTrail logs. This bucket should have a clear naming convention, such as `cloudtrail-logs-[account-id]`.
    - Apply the following best practices to the CloudTrail S3 bucket:
        - Enable MFA delete on the bucket to ensure that logs cannot be deleted without MFA.
        - Use S3 bucket policies to restrict access to the bucket. Only allow necessary IAM roles or users to access the logs.
        - Enable versioning on the S3 bucket to keep a history of log files and prevent accidental deletion.
        - Regularly back up the CloudTrail logs to another secure location, such as AWS Glacier or another secure storage solution.

6. **Regular Audits and Reviews**:
    - Conduct regular audits of AWS accounts to ensure compliance with these SOPs.
    - Review CloudTrail logs regularly to monitor for any suspicious or unauthorized activities.

### Conclusion:
Following these SOPs ensures that AWS accounts created on behalf of customers are secure, compliant, and managed according to best practices. Regular reviews and audits further ensure the ongoing security of these accounts.