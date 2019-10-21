Autonomy
=============

Introduction to Autonomy
************

As many of you probably know, autonomy is a very important and popular topic. Systems today are becoming more complex and as we continue asking systems due to more, engineers become more inclined to make systems 

An autonomous system usually consists of 4 components that function: perception, awareness, decision-making, and action. Each is briefly described:

* Perception: This component allows the system to "see" what is going on in its surroundings. This may be through what we consider our 5 senses (see, touch, taste, smell, hear) as well as another other artificial means (radar, infrared, etc.). 

* Awareness: Once the system can percept what your surroundings are, the system must be able to understand what is going on. Being able to "see" something and understand what is going on are most often two different tasks. For example, an autonomous car may see a pedestrian on the street; however, all the sensor has done is detect that there is a pedestrian on the street which is useful information in itself, but not as useful as understanding where the pedestrian is headed or trying to understand what it is trying to do.
 
* Decision making: This is the component that is generating the most buzz today and what people consider "artificial intelligence". How can we teach a robot to make decisions on what to do and not to do? For example, let us go back to the example of the autonomous car. When the autonomous car goes sees a pedestrian, what should it do? Depending on what the pedestrian is doing the car may decide to continue on or attempt a maneuver to avoid the pedestrian. Although this may seem like a simple problem to solve with different if/else logic for each scenario, the seemingly infinite possibilities of scenarios makes this problem impossible to solve with simply if/else statements.

* Action: This is component is what gets the most oohs/ahhs/Youtube video clicks in society. The action part of is the mechanism that allows systems to act on their decision. It could be as simple as running a computer program or as complex as flying from point A, delivery a package at point B, and landing at point C, all while avoiding traffic. This component is usually the physical hardware component of most systems.

The integration of all 4 components is one of the hardest challenge. Currently, all 4 components have various levels of maturity in the aerospace industry. Examples of interesting projects are the following:

* `Skyborg <http://www.airforcemag.com/Features/Pages/2019/July%202019/Skyborg-Eyeing-First-Flights-This-Summer.aspx>`_

* `AALIAS <https://www.lockheedmartin.com/en-us/products/sikorsky-matrix-technology.html>`_

* `AACUS <https://www.aurora.aero/wp-content/uploads/2017/12/AACUS-Press-Release_FINAL-12.13.pdf>`_


Let us look at two example systems to try to determine what parts of the system are which: the quadcopter that you will be using and a human being. The idea of having 4 different components of autonomy will be reinforced through the examination of these 2 systems. 

Quadcopter
-----------
Let's begin by looking at each of the systems onboard the quadcopter. We can classify all the systems onboard through the above introduced framework.

* Perception: IMU, GPS, Barometer, Magnetometer, Compass

* Awareness: Flight Computer, flight software

* Decision-Making: Flight computer, flight software, team's program

* Action: Motors, servos, mechanism

Human Being
-----------
Like many things that humans have designed and built, they are often modeled after the creator: human beings. You can distinctly define which parts of humans are which using the framework described above.

* Perception: Skin, eyes, ears, nose, mouth, tongue

* Awareness: Brain

* Decision-Making: Brain

* Action: All muscles, arms, legs, fingers, toes, etc.



Autonomy in ARC
***************

In the Aerospace Robotics Competition, the autonomy portion will always involve all the components. For example, for the 2019-2020 competition, all 4 components are involved. The perception is taken care by the GPS, the awareness is handled by the the autopilot, the decision making is handled by the team's computer program, and the autopilot and the action is carried out by the team design mechanism. 

As a note for future competition, ARC will continue to rotate between allowing teams to implement their own perception, awareness, decision-making, and/or action components. The 2019-2020 competition allowed teams to come up with the decision-making and action with the computer program and the drop mechanism design. 

2019-2020 Competition Specific Material: Planning
**********

In this year's competition, teams are asked create a computer program that allows the drone to traverse of a set of waypoints that are given to teams beforehand. **If you have not read the Programming section of the tutorial wiki, please read that before reading further.** 

There are many ways to introduce this topic; however, in the interest of making this understandable to high schoolers like you, we will condense it into format that will help teams in accomplishing the task.

The general problem that you are trying to solve is called the `"Traveling Salesman" problem <https://en.wikipedia.org/wiki/Travelling_salesman_problem>`_
.  This problem is a classic problem in the computer science and optimization world, and in essence comes down to "finding the path that takes the least amount of time for a person to travel to all the places it needs to go". 

One approach to go about accomplishing this is to iterate through all the different possible combinations of routes (keep in mind to make sure you start from the home base and return to the home base). In reality, this is not a realistic way as often times, the number of places you will need to visit is many times a very very large number and may take forever to go through every single combination. However, for this competition, we have designed it such that it is possible to do so.

Another way to go about accomplishing this task is to come up with a heuristic (or general idea/strategy) that should lead to a close to optimal route. This approach is often times used when the problem is so complex that we have a general idea that we know will give us the answer, but we have no guarantees that the answer will be the best one. For example, say you want to go from point A to point B. Point A is on the north and east side of Point B. Rather than going through Google Maps/Waze/Yahoo/your-choice-of-mapping-software to find the shortest route there, a strategy you could take is to take any road that takes you south and west, and hopefully get there (or close to there). This approach has surprisingly given many breakthroughs in computer science, as often times, you don't need to find the absolute optimal route to reach your destination/goal. Example heuristic ideas/strategies could involve going to the waypoint closest, or going to the waypoint that takes the least amount of time. The strategy can be more complex as well such as going minimizing the criss-crossing of routes or simply just taking the simplest route. 

We invite you to be creative and think hard on what are the best algorithms for this task! 

