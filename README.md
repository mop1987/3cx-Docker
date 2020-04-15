# 3cx-Docker
Docker Compose for 3CX Phone System

Run the following:

1. docker-compose up -d
2. docker exec 3cx timedatectl set-timezone <timezone>
3. docker exec -ti 3cx /usr/sbin/3CXWizard --cleanup


Access the initial setup with host IP and Port

X.X.X.X:5015/?v=2


You can find your timezone:  #timedatectl list-timezones 

example: #docker exec 3cx timedatectl set-timezone Europe/Paris

  
  
