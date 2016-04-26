## usage
```
sudo mkdir -p /artifactory/data && \
sudo mkdir /artifactory/logs && \
sudo mkdir /artifactory/backup && \
sudo mkdir /artifactory/etc && \
sudo chmod -R 755 /artifactory/data && \
sudo chmod -R 755 /artifactory/logs && \
sudo chmod -R 755 /artifactory/backup && \
sudo chmod -R 755 /artifactory/etc

docker run -d --name artifactory -p 8081:8081 -v /artifactory/data:/var/opt/jfrog/artifactory/data -v /artifactory/logs:/var/opt/jfrog/artifactory/logs -v /artifactory/backup:/var/opt/jfrog/artifactory/backup -v /artifactory/etc:/var/opt/jfrog/artifactory/etc jfrog-docker-reg2.bintray.io/jfrog/artifactory-oss
docker run -d --name artifactory -p 8081:8081 -v /artifactory/data:/var/opt/jfrog/artifactory/data -v /artifactory/logs:/var/opt/jfrog/artifactory/logs -v /artifactory/backup:/var/opt/jfrog/artifactory/backup -v /artifactory/etc:/var/opt/jfrog/artifactory/etc sklemmer/artifactory
```