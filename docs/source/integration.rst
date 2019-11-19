Integration/Assembly
=========================================

In this section, we will utilize a lot of material that has already been created for this specific purpose. Many of links are placed here. Please go through every webpage linked as most if not all links provide step-by-step instructions on how to integrate all the systems together.

Systems Overview
**************

The overall system diagram is shown in the below picture:

[show diagram]

All these individual components were introduced in the Drone 101 page. This diagram shows how the individual components are connected to each other. 

There are two operators: the pilot and the ground station operator. Contrary to popular belief, often times, automation requires **more people** to operate than non-automated systems (why? a good question to think about). The two operators interact with the quadcopter system differently: the pilot has direct control to the tactical/short-time-span actions while the ground station operator has a more strategic view of the system operation since it is ensuring that the quadcopter is executing its mission. 

The quadcopter operates by listening to the central autopilot which in this case is the APM or the Pixhawk. The autopilot sends signals to the ESC which translates it into a signal that motors can interpret. Depending on the time, a signal may be sent to the servo to actuate a mechanism. The battery powers all of these actions and is regulated through the power distribution board. 

As a reminder, teams are allowed to swap out parts for different systems not provided in the kit. Key questions to think about when considering that: 

- What are the advantages/disadvantages of swapping parts? Every part selection choice carries with it some pros and cons. Actually thinking through them is a useful exercise
- What additional systems can be attached on to allow for improved performance? Keep in mind, additional systems can be added during testing to improve the testing cadence
- How does the system choices influence operations? For example, when I'm flying, is there a way to know how much battery I have left without constantly looking at the ground station screen? Understanding system design choices and how it effects operations will go a long way in creating the optimal system for competition.

Systems Integration/Assembly
**************

Many of questions/instructions on how to integrate and assemble all the components have already been written out in the Arducopter documentation (see Software page for more details about Arducopter). If you are using the kit, all components of the kit are compatible with Arducopter. Please follow the below instructions to integrate all your components. Feel free to reach out to us (or even the people who wrote the tutorials!) if you have any specific questions.

Steps to first time flight with step-by-step instructions: http://ardupilot.org/copter/docs/initial-setup.html

Pixhawk details: http://ardupilot.org/copter/docs/common-pixhawk-overview.html

Pixhawk Wiring Instructions: http://ardupilot.org/copter/docs/common-pixhawk-wiring-and-quick-start.html

Receiver Connections: http://ardupilot.org/copter/docs/common-pixhawk-and-px4-compatible-rc-transmitter-and-receiver-systems.html

Connecting ESCs and Motors: http://ardupilot.org/copter/docs/connect-escs-and-motors.html

Flying preparation: http://ardupilot.org/copter/docs/flying-arducopter.html


