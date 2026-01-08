Deployment Steps
=
Step1. First we should have the AWS account created or with IAM User you can login
=
<img width="1920" height="949" alt="image" src="https://github.com/user-attachments/assets/7a0f976c-46df-4e23-8ace-fa49ade298e8" />

Step2.Launch EC2 Instance
=
1.Instance type: t2.micro

2.OS: Amazon Linux

3.Open ports:22 (SSH)

4.Custom application port (example: 32770)
<img width="1889" height="814" alt="Screenshot 2026-01-06 175928" src="https://github.com/user-attachments/assets/e1f5e737-1f95-4d1a-b409-326ae5d4ada9" />

Step3. Install Docker on EC2
=

sudo yum update -y

sudo yum install docker -y

sudo systemctl start docker

sudo systemctl enable docker 

sudo usermod -aG docker ec2-user

Step4. Build Docker Image
=
docker build -t nginx-app .

Step5. Run Docker Container
=
docker run -d -p 32770:80 nginx-app

Step6. Access the Application
=
Output:
=
Application deployed successfully using Nginx Docker container is LIVE & HEALTHY Hosted on AWS EC2 Accessible via public IP

✅ Application running in browser

<img width="1478" height="797" alt="Screenshot 2026-01-06 175829" src="https://github.com/user-attachments/assets/d18998fe-4292-45bf-b81b-6045497ccbf7" />

