# Day 4: Secure Web App Deployment
## Tasks Completed:
- Deployed Flask web app on private EC2 instance
- Configured Gunicorn to serve the Flask app with 2 workers on port 5000
- Installed and configured Nginx as a reverse proxy on the Bastion (public EC2)
- Set up Nginx to proxy requests to private EC2 Gunicorn app
- Verified web app access through Bastion public IP / domain
- Enabled VPC Flow Logs and sent them to CloudWatch for network monitoring

## Screenshots:
- Gunicorn running processes on private EC2
- Nginx configuration file snippet showing proxy_pass to private EC2
- Browser screenshot showing successful Flask app response
- Flow Logs configuration page in AWS console

## Notes:
- Binding Gunicorn to private IP restricts direct external access, enhancing security
- Nginx acts as a gateway to securely expose the app to public internet
- VPC Flow Logs help monitor and audit network traffic for troubleshooting and security
