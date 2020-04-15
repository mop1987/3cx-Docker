In order to use macvlan driver you will need to change the vSwitch security to allow promiscuous mode.

Also change the values in the compose file for the following to your relevant enviroment

- ipv4_address: IP
- parent: Host eth name
- subnet: CIDR
- gateway: IP


Run the following:

1. docker-compose up -d
2. docker exec 3cx timedatectl set-timezone [timezone]
3. docker exec -ti 3cx /usr/sbin/3CXWizard --cleanup

Note: The web interface does not detect the Macvlan adapter so you will not be able to complete setup wizard. To get around this issue, on step 3 above you must select option 2 (CLI) to enter the ip address manually when prompted and complete the wizard from the CLI.
