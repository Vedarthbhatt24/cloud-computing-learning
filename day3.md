# 🔐 Day 3: IAM Setup (Sept 12)

## 🧪 Hands-On Task
Created a new IAM user with programmatic access and assigned necessary policies.

### ✅ Steps Followed

1. **Opened IAM Console**
   - Navigated to AWS IAM service from the AWS Console.

2. **Created IAM User**
   - Username: `dev-user`
   - Access type: Programmatic access (Access Key ID & Secret Access Key generated)

3. **Assigned Permissions**
   - Attached existing policies:
     - `AmazonEC2FullAccess`
     - `AmazonS3FullAccess`
     - `IAMReadOnlyAccess`
   - Verified policy attachment and access levels.

4. **Configured Tags (Optional)**
   - Added tags for identification: `Project: CloudLearning`, `Owner: Vedarth`

5. **Downloaded Credentials**
   - Saved `.csv` file with access keys securely for CLI use.

## 📓 Notes
- IAM users with programmatic access are essential for CLI and SDK-based operations.
- Always follow the principle of least privilege—grant only necessary permissions.
- Consider enabling MFA and rotating access keys periodically for security.

---
