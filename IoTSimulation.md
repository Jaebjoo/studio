---
title: Studio 5 IoT Simulation
layout: default
description: Studio 5 IoT Simulation
---

## Studio 5 : 
# IoT Simulation

#### Client's Requests

The aim of this task is to simulate multiple IoT devices which have been installed in a fleet of trucks, connected to the IoT Central Platform.

The secondary aim is to explore the possibilities with Azure IoT Services.

#### Summary

Simulated Telemetry Data was received on the IoT Central and also a method was called on the device.

All the code was provided on Azure Learn.

This code and template can be modified to meet various use cases and scenarios.

#### Reflection

This was a beginners level exercise, however it widened my horizon on the possibilites of IoT services especially on Azure.

Before this exercise and the research into IoT, I had the understanding that IoT was limited to integrated household devices controlled by a central device that is voice controlled.

However the wide range of devices meant that IoT management services and small devices with their own small processing power could be integrated into many industries providing a unfathomable amount of data that could be used to increase productivity.

IoT could be integrated into:
* Manufracturing industry within factory machines on an assembly line
* Agricultural industry within crops to monitor farming conditions and respond to failing crops.
* Logistics industry within fleets of trucks and delivery drivers to reduce delays and boost delivery rates.
* Retail to monitor inventory levels in real time
* Medical industry to monitor patients' vital signs

![IoT](images\IoTSimulation\1IoT Architecture.png "IoT")

I have been made aware that there are free IoT platforms.
The advantage of the Azure Platform is that all of the Azure infrastructure can be fully integrated with the IoT Platform.
This includes the databases, security, other VMs, and most importantly, data analysis services (Stream Analytics). This allows the data to be processed into meaningful data.
It can also be integrated with machine learning services to compute this data into responses that are automated by algorithms.

#### Task Details

A device template needs to be created with a interface diaplaying what the device can store and print as data.

This can be created within Azure IoT Central.

![IoT](images\IoTSimulation\2IoTCentral.png "IoT")

The Azure IoT Central manages the IoT devices and connections.

These templates would be applied to a real device. 
Devices can also be added to IoT Central. 
Connection to the devices are managed with connection keys.

A Azure Maps Account can be created for free.

Demo Code can be taken from the Azure Learn pages.
Essentially, global location variables are added, with telemetry variables that are recorded by the device. The data is then routed to the IoT Central.

![IoT](images\IoTSimulation\3Telemetry.png "IoT")

![IoT](images\IoTSimulation\4Telemetry2.png "IoT")

Commands can also be sent to the device to initiate a process on the device.
In this case the device has been sent to a customer.

![IoT](images\IoTSimulation\5SendtoCustomer.png "IoT")

![IoT](images\IoTSimulation\6SendtoCustomer2.png "IoT")

This was a simple simulation for the IoT Devices sending telemetry data as well as calling methods on the device.