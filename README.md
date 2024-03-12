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

# Verify AWS Nuke Installation

<code>aws-nuke --help</code>

# Usage

Download/Create [config.yml](https://github.com/rushiranpise/aws-nuke/blob/main/config.yml) file in current directory

Get Access & Secret key from [here](https://us-east-1.console.aws.amazon.com/iam/home?region=us-east-1#/security_credentials/access-key-wizard)

<code>aws-nuke -c config.yml --access-key-id="key" --secret-access-key="key" --no-dry-run</code>
