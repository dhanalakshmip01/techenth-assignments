1. create two custom networks hr-net, emp-net using docker network create <network-name> command.
2. Run the emp1 contiainer in emp-net and get the ip address using docker inspect (docker run --name emp1 --network emp-net -d busybox sleep infinity)
3. Run the hr1 container in hr-net and try to check if hr1 is connecting to emp1 container or not.
4. Login to hr1 and ping emp1 ip address.
5. spin-up other container hr2 in hr-net and check is hr1 is connecting to hr2 or not. We can able to ping from hr2 to hr1 as both are in same network.
