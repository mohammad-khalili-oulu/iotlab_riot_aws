# Mini Project #1 for IoT Course

This project encompasses a series of essential steps:

Sensor Layer: Sensing the Environment
    Utilizing sensors available through IoT-Lab, our initial phase involved gathering crucial environmental data. We referred to the information provided in this link to facilitate this process. 
    Ref: https://github.com/iot-lab/openlab/blob/master/appli/iotlab_examples/tutorial/main.c

Network Layer: Multi-hop Transmission to the Border Gateway
    Once the data was collected, our focus shifted to the network layer. Employing techniques outlined in this repository, we established a multi-hop transmission method towards the border gateway.
    Ref: https://github.com/RIOT-OS/RIOT/tree/master/examples/gcoap

Network Layer: Sending Information to AWS Cloud
    Due to IoT-Lab's provision of IPv6 for external connections, we directed our data transmission towards AWS Cloud using strategies delineated in this repository.
    Ref: https://github.com/RIOT-OS/RIOT/tree/master/examples/gnrc_border_router

Application Layer: AWS Server Management of Collected Information
    Lastly, the AWS server was utilized within the application layer to efficiently manage and process the amassed data.
    Ref: https://www.youtube.com/watch?v=TUTqYEZZUdc

The subsequent sections provide detailed insights into each of these stages:
Sensor Layer

This phase concentrated on the foundational element of our project: capturing environmental data through a suite of sensors available via IoT-Lab. The integration process and utilization of resources from this repository formed the backbone of our data acquisition strategy.

## Board
This source code is used for the two first tutorials "First Steps" on the IoT-LAB Website.

It provides the following features:

    read sensors
    send a radio packet with CSMA MAC layer implementation
    blink LEDs (red, green, blue) with a 1hz period
    get nodes UID and match it with real node type and number using {UID: node} table
    i2c interact with control_node to get time


## Sensor Layer


The sensor layer serves as the foundational component for gathering environmental data crucial to this IoT project. This phase involves utilizing various sensors available through IoT-Lab to collect essential information about the environment.
Sensor Selection and Integration

The selection of sensors was meticulously executed to capture a comprehensive range of environmental parameters relevant to the project's objectives. Leveraging the information provided in this link, a selection of sensors including temperature, humidity, light sensors, and possibly others were integrated into the IoT infrastructure.
Data Collection and Processing

Each sensor was configured to collect specific data points according to predefined intervals or trigger conditions. The collected data was processed, cleaned, and formatted to ensure accuracy and consistency, ready for transmission through the network layer.
Implementation Details

The sensor integration process heavily relied on the capabilities and libraries offered by the IoT-Lab platform. This seamless integration enabled the acquisition of real-time data streams from multiple sensors, providing a robust foundation for subsequent layers to access and utilize this information.
Challenges and Solutions

During the implementation of the sensor layer, challenges such as sensor calibration discrepancies, synchronization issues among multiple sensors, or compatibility constraints might have been encountered. Solutions to these challenges were devised, ensuring reliable data collection and integrity.
Future Considerations

In future iterations or improvements, optimizing sensor performance, exploring additional sensor types for more comprehensive data collection, or implementing advanced algorithms for real-time data analysis could be considered to enhance the functionality and scope of the project.



