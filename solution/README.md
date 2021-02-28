docker pull infracloudio/csvserver:latest
docker pull prom/prometheus:v2.22.0
git clone https://github.com/infracloudio/csvserver.git
cd csvserver
cd solution/
vi gencsv.sh
sh gencsv.sh 
cat inputFile 
docker run -itd infracloudio/csvserver:latest bash
chmod 777 inputFile 
chmod 777 gencsv.sh 
docker run -itd -v /root/csvserver/solution/gencsv.sh:/csvserver/gencsv.sh:Z infracloudio/csvserver:latest bash
docker ps
docker exec -it 9b bash
docker stop 9b
docker rm  9b
history > README.md
