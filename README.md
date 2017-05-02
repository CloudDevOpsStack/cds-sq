# techo-sq
Techo SonarQube 


We need to clone the Repo as below 

git clone https://github.com/TechoDevOpsStack/techo-sq.git

Change the Directory to techo-sq

cd techo-sq

Run the below command to build the SonarQube on Docker Env as below 

docker build -t <IMAGE NAME> .

Create the Volume for SonarQube

docker volume create --name <SONARQUBE VOLUME NAME>

Create the container for Sonarqube by running below command

docker create -p <OUT SIDE PORT>:9000 --name <NAME FOR THE CONTAINER> -v <SONARQUBE VOLUME NAME>:/opt/sonarqube <IMAGE NAME>

Now start the container

docker start <CONTAINER_NAME>
