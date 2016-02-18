# mingo
Docker image for a MongoDB Cluster Manager automation agent


docker run -p 27000-27020:27000-27020 \
 -v /var/lib/docker/mingo/agent:/var/lib/mongodb-mms-automation \
 -v /var/lib/docker/mingo/data:/data \
 clusterdb/mingo:latest \
 --mmsBaseUrl=https://cloud.mongodb.com \
 --mmsGroupId=<GroupId> \
 --mmsApiKey=<ApiKey>
