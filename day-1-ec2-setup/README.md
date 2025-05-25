# Day 1: EC2 Launch & SSH Hardening

Tasks Completed:
- Launched new EC2 instance (Amazon Linux)
- Set up Security Group:
  - Allowed SSH (port 22 from my IP)
  - Allowed HTTP (port 80 from anywhere)
- Connected via SSH
- Created new user `newadmin`
- Hardened SSH:
  - Disabled root login
  - Disabled password auth
  - Set up key-based SSH for new user
Screenshots:
- EC2 running instance (Name, Type, Public IP)
- Terminal: SSH into EC2
- User creation steps
- `sshd_config` nano edit
- `systemctl restart sshd`
Important Notes:
- Remember to store `.pem` keys securely and move to home directory for easy access
