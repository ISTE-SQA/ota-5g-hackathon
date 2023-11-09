# ota-5g-hackathon

# Overview

TODO: Provide text

## OTA Prototype 

The OTA Prototype is a collection of software components developed as part of a bachelor's thesis to assess the impact on Quality of Service (QoS) for various Over-The-Air (OTA) update strategies. The prototype encompasses two different implemented versions: one without messaging (ota-tester-polling-intervals), and, one with messaging (ota-tester-with-broker). Additionally, it includes a load-generating component equipped with programmed simulation scenarios for updating car fleets of varying sizes.

For more detailed information about each component and the bachelor thesis, please visit https://github.com/PingPong3107/QoS-Analysis-of-OTA-Update-Approaches.

The services are implemented as Spring Boot Java Applications, while the load generator, which simulates the clients, utilizes Gatling and Scala.

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
