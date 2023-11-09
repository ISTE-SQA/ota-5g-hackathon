# OTA 5G Hackathon

The OTA 5G Hackathon Challenge aims at realizing a more realistic scenario for Over-the-Air Software Updates for cars and is part of [SofDcar Hackathon II](https://sofdcar.de/language/de/sofdcar-hackathon-ii).
In this repository, we collect all the necessary assets that are required to complete the challenge. 


## OTA Prototype 

<figure>
<p align="center">
  <img
  src="assets/architecture.png"
  alt="The beautiful MDN logo."
  width="550px">
</p>
  <figcaption>Figure 1: Architecture of the Prototype (source: Ingo Schwendinger)</figcaption>
</figure>
<br>
<br>

The OTA Prototype is a collection of software components developed as part of a bachelor's thesis to assess the impact on Quality of Service (QoS) for various Over-The-Air (OTA) update strategies.
The prototype encompasses two different implemented versions: one without messaging (ota-tester-polling-intervals), and one with messaging (ota-tester-with-broker).
Additionally, it includes a load-generating component equipped with programmed simulation scenarios for updating car fleets of varying sizes.

The services are implemented as Spring Boot Java Applications, while the load generator, which simulates the clients, utilizes Gatling and Scala.
An overview is give in Figure 1.
For more detailed information about each component and the bachelor thesis, please visit https://github.com/PingPong3107/QoS-Analysis-of-OTA-Update-Approaches.

## Challenge

In this challenge, we first deploy the already existing OTA prototype in a distributed manner across the 5G network of the Arena2036 and conduct 5G measurements. 
In the more advanced scenario, we introduce an edge cache and distribute the OTA prototype also across the cloud, while conducting new 5G measurements.
If interested, also deployment automation scripts can be provided.

### Default Scenario

* Distributed deployment of the prototype inside the Arena2036 5G network
* Deploy the server locally in one of the machines in the Arena2036 that is also connected to the 5G network. 
* Document the architecture as deployment diagram once the number of clients and the connection has been tested.
* Conducting 5G measurements
  * latency
  * throughput 
  * upload/download rate
  * gatling measurements 


### Advanced Scenario

* Introduce an edge cache between 5G clients and 5G edge server
* Move current 5G edge server to the cloud


### Automated Deployment Scenario

* Provide deployment scripts for the automated deployment of the distributed setup, e.g., using Ansible or TOSCA


## Hardware

We provide the following hardware.

### 5G Clients

* 5G driver (Windows recommended, https://www.tekmodul.de/download/quectel/drivers/Quectel_Windows_USB_Driver(Q)_NDIS_V2.7.6.zip)
* We provide 3 laptops (with drivers pre-installed?)
* We provide 3 5G TCUs
* TCUs are connected via USB to the laptops
* SIM cards with static IPs for entering the Nokia 5G Network included
* Participants may use their own devices (laptops with 5G TCU or 5G-capable smartphones) to increase the number of clients but need to install the drivers

### 5G Edge Server

* Laptop with Windows 11
* Connected via fourth 5G TCU
* Serves as edge in advanced use case
* **[action item]** Clarify how 5G edge server can connect to public cloud


### 5G Edge Core

* **[action item]** Clarify access with Nokia regarding measurements


### Cloud Server

* Virtual machine on Hetzner or bwCloud


## Contact

* Miles Stötzner
  * https://miles.stoetzner.de
  * miles.stoetzner@iste.uni-stuttgart.de
* Matthias Weiß
  * https://www.ias.uni-stuttgart.de/institut/team/Weiss-00019/
  * matthias.weiss@ias.uni-stuttgart.de