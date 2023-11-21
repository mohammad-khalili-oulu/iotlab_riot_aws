# Mini Project #1 for IoT Course

This project encompasses a series of essential steps:

Sensor Layer: Sensing the Environment
    Utilizing sensors available through IoT-Lab, our initial phase involved gathering crucial environmental data. We referred to the information provided in this link to facilitate this process. 
    Ref: https://github.com/iot-lab/openlab/blob/master/appli/iotlab_examples/tutorial/main.c

Network Layer1: Multi-hop Transmission to the Border Gateway
    Once the data was collected, our focus shifted to the network layer. Employing techniques outlined in this repository, we established a multi-hop transmission method towards the border gateway.
    Ref: https://github.com/RIOT-OS/RIOT/tree/master/examples/gcoap

Network Layer2: Sending Information to AWS Cloud
    Due to IoT-Lab's provision of IPv6 for external connections, we directed our data transmission towards AWS Cloud using strategies delineated in this repository.
    Ref: https://github.com/RIOT-OS/RIOT/tree/master/examples/gnrc_border_router

Application Layer: AWS Server Management of Collected Information
    Lastly, the AWS server was utilized within the application layer to efficiently manage and process the amassed data.
    Ref: https://www.youtube.com/watch?v=TUTqYEZZUdc

## Getting Started

To run this project, follow these steps:
1. Setting up IoT-Lab Account and SSH Key

    Create an Account: First, create an account on IoT-Lab.
    Generate RSA Key: Use the command ssh-keygen -t rsa to generate an RSA key.
    Add Key to IoT-Lab: Place the obtained key into your IoT-Lab account settings. Refer to this guide for detailed instructions.

Connect to the IoT-Lab website using the following SSH command:


ssh <user_id>@saclay.iot-lab.info

2. Clone RIOT Repository

Clone the RIOT repository using the command:


git clone https://github.com/RIOT-OS/RIOT

3. Navigate to RIOT Examples

Change the directory to RIOT's examples folder:


cd RIOT/examples

4. Clone This Project

Clone this project into the examples directory of RIOT:


git clone https://github.com/mohammad-khalili-oulu/iotlab_riot_aws.git


## Board
In this project, we utilized M3 boards of iot-lab.info and we got the required configuration from the [https://github.com/iot-lab/openlab/blob/master/platform/iotlab-m3/iotlab-m3_net.c]
It provides some required information and codes for reading sensors, sending a radio packet with CSMA MAC layer implementation, and getting nodes' UID (used to communicate with neighbor nodes).


## Sensor Layer
This phase concentrated on the foundational element of our project: capturing environmental data through a suite of sensors available via IoT-Lab. The integration process and utilization of resources from this repository formed the backbone of our data acquisition strategy.


The sensor layer serves as the foundational component for gathering environmental data crucial to this IoT project. This phase involves utilizing various sensors available through IoT-Lab to collect essential information about the environment.
Sensor Selection and Integration

The selection of sensors was meticulously executed to capture a comprehensive range of environmental parameters relevant to the project's objectives. Leveraging the information provided in this link, a selection of sensors including temperature ("42.5 + value / 480.0" was used to convert the sensed value to a centigrade degree), humidity ("value / 4096.0"), light sensors (in lux).

## Network layer 1




## Network layer 2
