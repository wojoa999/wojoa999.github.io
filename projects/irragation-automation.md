---
layout: project
type: project
image: img/irraz.png
title: "Irrigation Automation"
date: 2024
published: true
labels:
  - Ignition Perspective
  - DXM Software
  - Irrigation
summary: "Developing a remote-access SCADA system to automate crop irrigation, monitoring soil moisture, and valve control via mobile and web interfaces."
---

<div class="text-center p-4">
  <img width="300px" src="../img/banner.jpg" class="img-thumbnail" >
  <img width="400px" src="../img/software.png" class="img-thumbnail" >
</div>

## Project Overview
The purpose of this project was to automate the irrigation system for a better crop management system. The primary goal was to make crop management more efficient by creating a system that would allow the irrigation schedule to be monitored by a mobile device or computer rather than manually checking. A new system would allow the team to track the moisture in the ground, weather, and the capability to check the pressure remotely. 

The central and main valves are another critical focus of the automation system. This would allow the central valves to be opened and closed remotely, reducing the need for on-site personnel to come into work over the weekend to shut off valves if an issue such as a mainline break or an overflowing reservoir occurs. The system will simplify the irrigation process and allow crops to get the desired amount of water.

## Technical Implementation
The project involved establishing a network gateway and integrating Banner Engineering's wireless hardware with SCADA software.

* **Ignition Perspective:** Utilized to design a user interface for real-time monitoring and remote valve controls.
* **Banner Engineering DXM:** Programmed using DXM software to handle the backend logic for wireless communication between devices.
* **Wireless Mesh Network:** Configured wireless controllers as both end-nodes and repeaters to ensure signal coverage across the farm.

## My Contributions
 My role focused on the programming, network optimization, and field deployment of the automation hardware.

* **Controller Programming:** I programmed the Banner Engineering DXM controllers, establishing the communication logic between the field sensors and the gateway.
* **Network Testing:** I conducted range testing to identify signal dead zones. Based on this data, I optimized the locations for repeaters for the optimal connection.
* **Field Deployment:** I engaged in the deployment of the control boxes at various water sources, verifying that the hardware-to-software handshake functioned correctly under real-world conditions.
* **System Integration:** I gained proficiency in Ignition Perspective, ensuring that the data collected by the boxes was accurately represented on the user interface.
