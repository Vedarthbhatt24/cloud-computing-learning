# 🔐 Day 5: Configure Security Groups

## 🧪 Hands-On Task
Modified inbound and outbound rules in a security group to allow SSH and HTTP access.

### ✅ Steps Followed

1. **Opened EC2 Console**
   - Navigated to the “Security Groups” section under EC2.

2. **Selected Existing Security Group**
   - Group Name: `dev-instance-sg`
   - Associated with previously launched EC2 instance.

3. **Modified Inbound Rules**
   - Added rule for SSH:
     - Type: SSH
     - Protocol: TCP
     - Port Range: 22
     - Source: My IP
   - Added rule for HTTP:
     - Type: HTTP
     - Protocol: TCP
     - Port Range: 80
     - Source: Anywhere (0.0.0.0/0)

4. **Modified Outbound Rules**
   - Verified default rule: All traffic allowed
   - No changes needed for basic web access

5. **Saved Changes**
   - Confirmed rules applied and instance accessible via SSH and HTTP

## 📚 Additional Learning Resources
- [HOW TO Configure SECURITY GROUPS in AWS? | AWS ...](https://www.youtube.com/watch?v=qdHkGx0uFMQ) – Quick walkthrough of security group setup and rule editing.
- [Amazon EC2 Security Groups Tutorial](https://www.youtube.com/watch?v=nA3yN76cNxo) – Explains how security groups control traffic and how to apply them.
- [AWS EC2 Security Groups: Essential Guide](https://www.youtube.com/watch?v=mdby1-j2w1k) – Covers theory and hands-on demo for rule configuration.
- [AWS Security Groups Simply Explained: A Step-by-Step ...](https://www.youtube.com/watch?v=uYDT2SsHImQ) – Breaks down inbound/outbound rules with examples.
- [Creating and deleting Security groups in AWS Using Console](https://www.youtube.com/watch?v=dmgl2W2HNwE) – Shows how to create, edit, and delete security groups.
- [AWS Security Groups | Inbound Rule and Outbound Rule ...](https://www.youtube.com/watch?v=CW_3D1tL3_I) – Deep dive into protocols, ports, and rule logic.

## 📓 Notes
- Security groups act as virtual firewalls—stateful by design.
- Inbound rules define what traffic can reach your instance.
- Outbound rules define what traffic can leave your instance.
- Always restrict SSH access to your IP for security.

---
