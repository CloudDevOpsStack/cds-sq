# techo-sq
Techo SonarQube 


We need to clone the Repo as below 

git clone https://github.com/TechoDevOpsStack/techo-sq.git

Change the Directory to techo-sq

cd techo-sq

Run the below command to build the SonarQube on Docker Env as below 

docker build -t <IMAGE_NAME> .

Create the Volume for SonarQube

docker volume create --name <SONARQUBE_VOLUME_NAME>

Create the container for Sonarqube by running below command

docker create -p <OUT_SIDE_PORT>:9000 --name <NAME_FOR_THE_CONTAINER> -v <SONARQUBE_VOLUME_NAME>:/opt/sonarqube <IMAGE_NAME>

Now start the container by running below command 

docker start <CONTAINER_NAME>
