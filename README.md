# Introduction
This is a diagram template created for building software architectures with [Zephyr RTOS](https://docs.zephyrproject.org/latest/introduction/index.html)'s [ZBUS](https://docs.zephyrproject.org/latest/services/zbus/index.html) service.

_Below is an example showing how a software architecture diagram looks like when created using this template._
![Diagram connection example](https://github.com/Batto1/Zephyr-ZBUS-Architecture-Diagram-Template/assets/76911536/8b9c92c1-c340-403b-a75d-af7959faf649)

## About
I had the following needs after developing many versions of congested, unexpandable, non-modular and unsafe code for a project:
1. An easier and safer way to develop code with RTOS since there occurs constant time consuming considerations for race conditions of resources and synchronisation between threads throughout the whole development process of the software. This also increases the complexity as the project grows.
2. A convenient and simple way to be able to design a complete software architecture visually before beginning to code, which also can guide the whole development process directly. This architecture should be able to convey both higher or lower level design as required throughout the phases of a project.

1st need was met by incorporationg the use of ZBUS which is a lightweight and flexible software bus that provides the desired abstraction for ease of development. _See more on [here](https://docs.zephyrproject.org/latest/services/zbus/index.html)._

2nd need was met by designing this software architecture template, which was made possible with incorporation of ZBUS.

* If you have similar needs, you need to put effort for learning ZBUS but you might not need to put more effort for creating a diagram template for designing software architectures. 
* You can use the architecture diagram template without incorporating the use of ZBUS, although its convenience would depend on how you'd use it. 
  
Note: If you have any feedback, a modification request for the architecture template or noticed a mistake, please let me know by creating an issue or reaching me using the contact information I've provided below.


## Example Project
There is an [example architecture](https://github.com/Batto1/Zephyr-ZBUS-Architecture-Diagram-Template/blob/730daa6ae7a3276a20c41233fdf4c2badc79a6ec/Example%20Architecture%20of%20a%20Real%20IoT%20Project.pdf) of a real IoT project provided in this repo. Since this is of an actual work project, most of the information is hidden for confidentiality. But this only conceals the algorithms and characteristics specific to the project, and is still useful for demonstrating how algorithms and flow of the tasks are designed while ZBUS is employed.

Notice: This is only a snapshot of the project's SW architecture which was ongoing. It may have mistakes or might be incomplete. Developing software from the architecture was still ongoing while this repo was uploaded. If you have any feedbacks or noticed a mistake, please let me know by creating an issue or reaching me using the contact information I've provided below.

# Getting Started
## Prerequisites
* [draw.io](https://draw.io/) for opening the [ZBUS Architecture Template](https://github.com/Batto1/Zephyr-ZBUS-Architecture-Diagram-Template/blob/730daa6ae7a3276a20c41233fdf4c2badc79a6ec/SW%20Architecture%20With%20ZBUS%20Diagram%20Template%20v1.19.0.drawio). You can also download the [draw.io desktop app](https://github.com/jgraph/drawio-desktop/releases/tag/v22.1.16).
* Familiarity with [ZBUS](https://docs.zephyrproject.org/latest/services/zbus/index.html).

## Usage
Build your architecture using the blocks in the template in draw.io. You can check the [example architecture](https://github.com/Batto1/Zephyr-ZBUS-Architecture-Diagram-Template/blob/730daa6ae7a3276a20c41233fdf4c2badc79a6ec/Example%20Architecture%20of%20a%20Real%20IoT%20Project.pdf) for further reference.

## Contact
[LinkedIn](https://www.linkedin.com/in/hikmet-batuhan-g%C3%B6rg%C3%BCl%C3%BC-3758581b5)

## Credits
* This template would have no purpose to be created if ZBUS didn't exist. I'd like to thank the ZBUS creator [Rodrigo Peixoto](https://github.com/rodrigopex).
* [Kerem Sarı](https://github.com/KeremSAR): Created a demo how initial version of the template could look like and we've built the example architecture together.  
