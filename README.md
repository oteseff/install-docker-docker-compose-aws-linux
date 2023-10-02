# install-docker-docker-compose-aws-linux
Steps to install docker and docker-compose in AWS Linux

## Install docker
`sudo yum install -y docker`
`sudo systemctl start docker`
`sudo systemctl enable docker`
`sudo usermod -a -G docker ec2-user`

## Sign out and back in
`docker version`

## Install docker-compose
`sudo curl -L https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -m) -o /usr/local/bin/docker-compose`
`sudo chmod +x /usr/local/bin/docker-compose`
`docker-compose version`
