# aws-nuke
Script for using AWS Nuke

# Install AWS Nuke on Ubuntu / WSL

<code>sudo apt update && sudo apt upgrade -y
sudo apt install tar wget -y
wget https://github.com/rebuy-de/aws-nuke/releases/download/v2.25.0/aws-nuke-v2.25.0-linux-amd64.tar.gz
tar -xvf ./aws-nuke-v2.25.0-linux-amd64.tar.gz aws-nuke-v2.25.0-linux-amd64 
chmod u+x aws-nuke-v2.25.0-linux-amd64
sudo mv aws-nuke-v2.25.0-linux-amd64 /usr/local/bin/aws-nuke
</code>

# Install AWS Nuke on Windows

1. Download and Extract Zip [link](https://github.com/rebuy-de/aws-nuke/releases/download/v2.25.0/aws-nuke-v2.25.0-windows-amd64.zip)
2. Go to the extracted folder eg. aws-nuke-v2.25.0-windows-amd64
3. Open CMD in the current folder

# Verify AWS Nuke Installation

<code>aws-nuke --help</code>

# Usage

1. Download/Create/Edit [config.yml](https://github.com/rushiranpise/aws-nuke/blob/main/config.yml) file in current directory
2. Set Account Alias [here](https://us-east-1.console.aws.amazon.com/iam/home#/home)
3. Get Access & Secret key [here](https://us-east-1.console.aws.amazon.com/iam/home?region=us-east-1#/security_credentials/access-key-wizard)
4. Run the below command to nuke all

<code>aws-nuke -c config.yml --access-key-id="your-access-key" --secret-access-key="your-secret-key" --no-dry-run</code>
