# 🔐 Task 14: Linux Server Hardening & Secure Configuration

## 📌 Objective
To secure a Linux system by applying server hardening techniques and reducing attack surface.

---

## ✅ Steps Performed

### 1️⃣ User Account Review
- Reviewed /etc/passwd
- Identified normal users (UID ≥ 1000)
- Verified no unnecessary privileged accounts

### 2️⃣ Sudo Privilege Restriction
- Checked sudo group membership
- Confirmed only authorized user has sudo access
- Maintained Principle of Least Privilege

### 3️⃣ SSH Hardening
- Disabled root login (PermitRootLogin no)
- Disabled password authentication
- Enabled key-based authentication
- Generated ed25519 SSH keys
- Secured .ssh directory permissions

### 4️⃣ System Updates
- Updated system packages
- Verified latest security patches installed

### 5️⃣ Firewall Configuration
- Installed and enabled UFW
- Default deny incoming traffic
- Allowed only SSH (port 22)

### 6️⃣ Service Hardening
- Reviewed enabled services
- Disabled unnecessary services (Docker, ModemManager)
- Reduced system attack surface

### 7️⃣ File Permission Security
- Secured /etc/shadow
- Set strict permissions for SSH keys

### 8️⃣ Log Monitoring
- Reviewed SSH logs using journalctl
- Verified no suspicious authentication attempts
