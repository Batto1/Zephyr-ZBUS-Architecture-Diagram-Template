# Introduction
This is a diagram template created for building software architectures with [Zephyr RTOS](https://docs.zephyrproject.org/latest/introduction/index.html)'s [ZBUS](https://docs.zephyrproject.org/latest/services/zbus/index.html) service.

_Below is an example showing how the architecture diagram template looks like._
![Diagram connection example](https://github.com/Batto1/Zephyr-ZBUS-Architecture-Diagram-Template/assets/76911536/8b9c92c1-c340-403b-a75d-af7959faf649)

## About
I had the following needs after developing many versions of congested, unexpandable, non-modular and unsafe code for a project:
1. An easier and safer way to develop code with RTOS since there occurs constant and time consuming considerations for race conditions of resources and synchronisation between threads throughout the whole development process of the software. This also increases the complexity as the project grows.
2. A convenient and simple way to be able to design a complete software architecture visually before beginning to code, which also can guide the whole development process directly. This architecture should be able to convey both higher or lower level design as required throughout the phases of a project, such as what and how many threads are in use and what task they accomplish. Without a visual representation, your architecture will be embedded in the code and your architecture will probably be designed poorly at the end. Also, your code will probably be very congested, non-modular, hard to maintain and harder for other people to understand.

1st need was met by incorporationg the use of ZBUS which is a lightweight and flexible software bus that provides the desired abstraction for ease of development. _See more on [here](https://docs.zephyrproject.org/latest/services/zbus/index.html)._

2nd need was met by designing this software architecture template, which was made possible with incorporation of ZBUS.

* If you have similar needs, you need to put effort for learning ZBUS, but you might not need to put more effort for creating a diagram template for designing software architectures. 
* You can use the architecture diagram template without incorporating the use of ZBUS, although its convenience would depend on how you'd use it. 
  
Note: If you have any feedback, a modification request for the architecture template or noticed a mistake, please let me know by creating an issue or reaching me using the contact information I've provided below.


## Example Project
There is an [example architecture](https://github.com/Batto1/Zephyr-ZBUS-Architecture-Diagram-Template/blob/730daa6ae7a3276a20c41233fdf4c2badc79a6ec/Example%20Architecture%20of%20a%20Real%20IoT%20Project.pdf) of a real IoT project provided in this repo. Since this is of an actual work project, most of the information is hidden for confidentiality. But this only conceals the algorithms and characteristics specific to the project, and is still useful for demonstrating how algorithms and flow of the tasks are designed while ZBUS is employed.

**Notice:** This is only a snapshot of the project's SW architecture which was ongoing. It may have mistakes or might be incomplete. Developing software from the architecture was still ongoing while this repo was uploaded. If you have any feedbacks or noticed a mistake, please let me know by creating an issue or reaching me using the contact information I've provided below.

# Getting Started

## Usage
Build your architecture using the blocks in the template in draw.io. You can check the [example architecture](https://github.com/Batto1/Zephyr-ZBUS-Architecture-Diagram-Template/blob/730daa6ae7a3276a20c41233fdf4c2badc79a6ec/Example%20Architecture%20of%20a%20Real%20IoT%20Project.pdf) for further reference.

## Tips
**How Detailed Should Your Architecture Diagram Be?**
* You can design your architecture in high-level where you make the naming of the processes more human readable rather than getting into technical details. Then you keep the technical details in some other documents or implement them as modules as a reference when starting the development for your project.
* You can design your architecture in low-level where you name and explain processes in more detail, even referencing the namings in the code. 
* (Recommended) You can design your architecture in both high-level and low-level. For instances where you can hide details and perform abstraction for individual processes, use high-level explanations for processes, explain lower-level details elsewhere. For instances where you need to show lower-level details for clarity, detail the explanations for processes as you need. 

|   Tip   | Pros          |     Cons      |
|-------------| ------------- | ------------- |
|    High-level design     | • Architecture diagram looks concise. <br> • Lower-level changes in the architecture don't need to be synced into architecture diagram | • Important low-level implementation details don't exist in the architecture diagram.   |
|    Low-level design     | • Most of the development of the code will be possible by referencing from the architecture diagram.  | • Architecture diagram looks complex and overwhelming. <br>  • Architecture diagram is hard to maintain and incorporate changes. <br>  • Architectural changes whether it be high or low level is very hard. |
|    Both high and low-level design (recommended)    | • Pros of both high and low level design choice depending on their weighted incorporation. <br> • Architecture captures both high level picture and incorporates necessary low level details. | • Cons of both high and low level design choice depending on their weighted incorporation. <br> • Architecture diagram might look complex and crowded depending on the incorporation of lower level detail. |

**About The Process of Designing The Architecture**
* Design a high level architecture based on your requirements. As you start to dive deep into lower level problems and solutions, requirements will also be developed into lower levels. Update your architecture as you progress. After you crack lower level implementation details, incorporate them in the architecture or document their solution design elsewhere based on how you'd like your architecture diagram to look like. 
* As you progress from higher level to lower level solutions, your vision on the architecture will develop and what architecture represents in the actual code will be more clearer.
* Don't start coding for your actual project until you feel that every core high level and lower level solution is explored. This doesn't mean that you shouldn't start coding, you should be coding modules or be coding for exploring solutions. This will help to reduce the probability that there will be a major change occuring after you started coding and you will have a better vision how the architecture diagram will be converted to the actual code.

**Collaboration Tips**
* If you're working with a team, involve every necessary person that will be in the development process, in architecture diagram design so that everyone will gain a familiarity and the architecture diagram will look less overwhelming.
* The diagram itself isn't enough for conveying every low-level implementation detail so everyone need to be consulting and communicating to each other about how to code referencing the architecture diagram in coding phase.

## Prerequisites
* [draw.io](https://draw.io/) for opening the [ZBUS Architecture Template](https://github.com/Batto1/Zephyr-ZBUS-Architecture-Diagram-Template/blob/730daa6ae7a3276a20c41233fdf4c2badc79a6ec/SW%20Architecture%20With%20ZBUS%20Diagram%20Template%20v1.19.0.drawio). You can also download the [draw.io desktop app](https://github.com/jgraph/drawio-desktop/releases/tag/v22.1.16).
* Familiarity with [ZBUS](https://docs.zephyrproject.org/latest/services/zbus/index.html).

## Contact
[LinkedIn](https://www.linkedin.com/in/hikmet-batuhan-g%C3%B6rg%C3%BCl%C3%BC-3758581b5)

## Credits
* This template would have no purpose to be created if ZBUS didn't exist. I'd like to thank the ZBUS creator [Rodrigo Peixoto](https://github.com/rodrigopex).
* [Kerem Sarı](https://github.com/KeremSAR): Created a demo how initial version of the template could look like and we've built the example architecture together.  
