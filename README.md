# ota-5g-hackathon

# Overview

TODO: Provide text

## OTA Prototype 
Answer questions like: 
What are the main components in the prototype? 
How it is currently envisioned to be deployed? >> Kube files  
https://github.com/PingPong3107/QoS-Analysis-of-OTA-Update-Approaches

## Hardware

### Laptops as 5G Clients
* 5G driver (Windows recommended, https://www.tekmodul.de/download/quectel/drivers/Quectel_Windows_USB_Driver(Q)_NDIS_V2.7.6.zip)
* We provide 3 laptops (with drivers pre-installed?)
* We provide 3 5G TCUs
* TCUs are connected via USB to the laptops
* SIM cards with static IPs for entering the Nokia 5G Network included
* Participants may use their own devices (laptops with 5G TCU or 5G-capable smartphones) to increase the number of clients but need to install the drivers

### Laptop as Server
* Windows 11 operating system
* Connected via fourth 5G TCU
* Serves as edge in advanced use case

### Edge Core?
Clarify access with Nokia regarding measurements


# New Features

## Default Scenario Features

* Distributed local deployment for the 5g clients
Deploy the server locally in one of the machines in the arena that is also connected to the 5g network. 
TODO: Create a deployment diagram once the number of clients and the connection has been tested. 

* Conducting 5g measurements

What? 
latency
throughput 
upload/download rate
gatling measurements 

How?
describe a protocol/or activity diagram



## Advanced Features

* Introducing an Edge Cache

* Moving server to a cloud backend
Firewall? 
CS cluster connected to arena, OR server on the public cloud.
