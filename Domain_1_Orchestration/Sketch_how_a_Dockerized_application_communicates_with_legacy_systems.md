# How a Dockerized application communicates with legacy systems
**Use macvlan networks**
> Some applications, especially legacy applications or applications which monitor network traffic, expect to be directly connected to the physical network. In this type of situation, you can use the `macvlan` network driver to assign a MAC address to each container’s virtual network interface, making it appear to be a physical network interface directly connected to the physical network. In this case, you need to designate a physical interface on your Docker host to use for the `macvlan`, as well as the subnet and gateway of the `macvlan`. You can even isolate your `macvlan` networks using different physical network interfaces. 

## Official Docker Documentation
[Use macvlan networks](https://docs.docker.com/network/macvlan/)

[Understanding Docker Container Communication](https://docs.docker.com/engine/userguide/networking/default_network/container-communication/)  
