    1  docker pull infracloudio/csvserver:latest
    2  docker pull prom/prometheus:v2.22.0
    3  git clone https://github.com/infracloudio/csvserver.git
    4  cd csvserver/
    5  cd solution/
    6  vi gencsv.sh
    7  sh gencsv.sh 
    8  cat inputFile 
    9  docker run -itd infracloudio/csvserver:latest bash
   10  chmod 777 inputFile 
   11  chmod 777 gencsv.sh 
   24  docker run -itd -v /root/csvserver/solution/gencsv.sh:/csvserver/gencsv.sh:Z infracloudio/csvserver:latest bash
   25  docker ps
   26  docker exec -it 9b bash
   27  docker stop 9b
   28  docker rm  9b
   49  history > README.md
