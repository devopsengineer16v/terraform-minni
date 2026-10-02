<img width="887" height="175" alt="image" src="https://github.com/user-attachments/assets/d5f15cb0-c0b8-461f-b665-e9c178d271d8" /># terraform-minni
Terraform installation: ubuntu

https://developer.hashicorp.com/terraform/install //Terraform installation link//

wget -O - https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(grep -oP '(?<=UBUNTU_CODENAME=).*' /etc/os-release || lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install terraform

**AWS installation:**

1.
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

2.
unzip awscliv2.zip
sudo apt install unzip
unzip awscliv2.zip

3.
sudo ./aws/install --bin-dir /usr/local/bin --install-dir /usr/local/aws-cli --update


4.
ubuntu@ip-172-31-39-103:~$ aws --version
aws-cli/2.34.45 Python/3.14.4 Linux/7.0.0-1004-aws exe/x86_64.ubuntu.26

python is pre-installed -see, so no need to install python -pre-requisite

5.aws configure

Tip: You can deliver temporary credentials to the AWS CLI using your AWS Console session by running the command 'aws login'.

AWS Access Key ID [None]: 
AWS Secret Access Key [None]:




























