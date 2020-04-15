In order to use macvlan driver you will need to change the vSwitch security to allow promiscuous mode.

Also change the values for the following to your relevant enviroment

- ipv4_address: IP
- parent: Host eth name
- subnet: CIDR
- gateway: IP


Run the following:

1. docker-compose up -d
2. docker exec 3cx timedatectl set-timezone [timezone]
3. docker exec -ti 3cx /usr/sbin/3CXWizard --cleanup


Access the initial setup with host ipv4_address and port

X.X.X.X:5015/?v=2


