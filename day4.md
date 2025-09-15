# 🚀 Day 4: Launch EC2 Instance (Sept 13)

## 🧪 Hands-On Task
Launched a Linux-based EC2 instance and connected via SSH.

### ✅ Steps Followed

1. **Opened EC2 Console**
   - Navigated to EC2 dashboard from AWS Console.

2. **Launched New Instance**
   - AMI: Amazon Linux 2023 (Free Tier eligible)
   - Instance type: `t2.micro`
   - Key pair: Created new key pair `vedarth-key.pem`
   - Security group: Allowed inbound SSH (port 22) from my IP

3. **Instance Configuration**
   - Storage: Default 8 GB
   - Network: Default VPC and subnet
   - Tags: `Name: DevInstance`, `Project: CloudLearning`

4. **Connected via SSH**
   - Used terminal with command:
     ```bash
     ssh -i "vedarth-key.pem" ec2-user@<Public-IP>
     ```
   - Verified connection and ran basic Linux commands (`uname -a`, `df -h`, `uptime`)

## 📓 Notes
- Always download and store `.pem` file securely—cannot be retrieved again.
- Security group rules must be precise to avoid access issues.
- SSH access confirms instance readiness for future deployments.

---
