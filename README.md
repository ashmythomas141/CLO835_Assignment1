# CLO835_Assignment1

1. Running terraform
   `terraform init`
   `terraform validate`
   `terraform plan`
   `terraform apply`
3. github workflow add main.yml
### Steps
 ssh -i keyname IP

sudo yum update -y
$ sudo yum install docker -y
$ sudo systemctl start docker
$ sudo systemctl status docker
sudo usermod -aG docker ec2-user

sudo systemctl start docker

aws configure
vi ~/.aws/credentials

docker pull image db URI
docker pull image app

# Stop all running containers
docker stop $(docker ps -q)

# Remove all stopped containers
docker rm $(docker ps -a -q)

docker network create  -d bridge test 


aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 257315592381.dkr.ecr.us-east-1.amazonaws.com

docker run -d --network=test -e MYSQL_ROOT_PASSWORD=pw url of app
export DBHOST=172.17.0.2
export DBPORT=3306
export DBUSER=root
export DATABASE=employees
export DBPWD=pw
export APP_COLOR=blue

  docker run -p 8081:8080 --name blue -e DBHOST=$DBHOST -e DBPORT=$DBPORT -e DBUSER=$DBUSER -e DBPWD=$DBPWD -e APP_COLOR=blue --network=test url of db_image
docker ps
We need to go inside one of the containers with this cmd:
docker exec -it <blue/pink/lime> /bin/bash
 And then install ping in that container using:

apt-get update
apt-get install iputils-ping

ping pink(The other container's name)

### Assignment2
