Programming
=============

Introduction
*********

Programming is needed to accomplish the tasks to compete in the autonomous portion of the competition. We will provide a very *brief* overview of what programming is in a nutshell. **Please refer to the additional resources for actual coursework, this page only serves as a brief overview.**

In a nutshell, computer programming is developing a set of instructions and encoding them into the computer such that the computer can carry out the instructions. The set of instructions or algorithms dictate how the computer will carry them out, and the translation/encoding makes the instructions understandable to the computer. From the description given above, 

Many people often fall into the trap of diving right into the actual coding of the computer rather than firmly developing the set of instructions or algorithms that it wants the computer program to execute. This is often times a trap as the programmer will most likely end up spending more time programming if they dove right into the coding compared to someone who spends some upfront time to fully define the instructions to which they want the computer or system to carry out. 

This section is divided into two sections: Algorithms and Software Engineering. The algorithms section is intended to help teams figure out how to properly fully define the instruction set they want the computer to carry out. The Software Engineering portion will dive into the the coding of the computer. 

It is impossible to teach everything there is about computer programming in a single web-page, so this page summarizes the important points that teams should understand and utilize to compete in the competition. Additional resources are given in the Resources section.

Finally, a walkthrough of the example code is given in the 2019-2020 Competition Specific Material section. The hope is that teams can use that example code as a starting point for developing their own path-planning code as outlined in the competition rules.

Algorithms
**********
Algorithms are defined as a set of instructions that allows the computer to accomplish its goal. These sets can be vary from very complex algorithms such as machine learning to AI or can be as simple as a calculation of a formula.

A set of instructions can be broken down into 3 different components. All instructions are formed by a combination of these three. The different types of instructions:

* Command: This is pretty self explanatory as it forms is what really executes the instructions. This is one of the simplest form of an algorithm as it essentially tells the computer specifically what action to take.
* Conditional: A conditional allows commands to occur only if certain conditions are fulfilled. Most often called if/else statements, a computer will run a command defined in the if portion of the code if the condition is satisfied; otherwise, it will run the else statements. There also exists if/elseif/else where you can define multiple conditions to check for when the computer is deciding what to do. If there are many different conditions you want to check, a "switch" statement may be more useful. 
* Loops: This construct allows command(s) to be carried out multiple times in a row. The number of times is dependent on how the loop is set up. There are two types of loops: for loops and while loops. In for loops, you specify how many times the command should be repeated. While loops allow you to combine both a conditional and a loop: the command(s) will continue to be executed until a certain condition is met or a condition is not being met.

These three combined can form an algorithm. Let's look at an example: a recipe. 
In a recipe, you have a set of instructions that you have to follow. For example, if the recipe calls for two eggs to be added into a bowl, that would be an example of a command. A conditional could be that if the dough is not clumping as much it should be, add water. The condition here is checking the clumping-ness of a dough and the action if the condition is not satisfied as adding the water. An example of a loop is putting something into the oven until it rises. Although you may not explicitly be continually adding stuff into the oven (keeping say the batch in the oven could itself be a command), the while loop conditional can be the status of how much the batch has "risen". 

When developing an algorithm, the primary strategy is to see if you can apply these 3 components in certain ways that allow you to accomplish the task that you want carried out by the computer program. Thinking through how these components can be combined and taking advantage of the pros and cons will allow great algorithms to be developed. 

Software Engineering
********************
Software engineering is at its core the **translation of instructions to something a computer can understand**. Once the set of instructions or algorithms is defined above, the usage of computer languages is relatively straight forward. 

We will not go over the specifics of how to program here; the additional resources provided will do  a much better job than what we can do here. However, some key points and tools will be provided here so that teams can get started on programming as well as some tips.

Programming Languages
----------
Similar to how there are many languages that we humans can use to talk to one another, there are also many different computer languages that allow humans to program computers. Below are some examples. For this competition, we highly recommend the use of Python due to its extensive support, usefulness, and simplicity. Additional resources to learn Python are given in the additional resources section.

* Python: https://www.python.org/
* C++: http://www.cplusplus.com/
* Java: https://www.java.com/en/
* Perl: https://www.perl.org/
* Fortran: https://www.fortran.com/
* MATLAB / Octave: https://www.gnu.org/software/octave/

From this point on, we will assume that the team will be programming in Python. 


Compilers/IDEs/Editors
----------
Code is a human-readable version of a set of instructions that you want to give to a computer. However, the computer cannot read code; it needs to be converted or "compiled" to a format that computers can. There are two ways we can do it: interpreters and compilers. Interpreters are computer programs designed to read line by line your computer code and send the computer the translation line by line. Compilers on the other hand convert your entire script into something machine-readable. The execution of that program is done later and in another process. Python is an example programming language that is interpreted, and C++ is an example of a programming language that is compiled.

Many computer applications called Integrated Development Environemnt (IDE) /Editors exist to help with coding/compiling/running process. Below are some great examples that we recommend teams use to help with their coding:

* `VS Code <https://code.visualstudio.com/>`_
* `Sublime Text <https://www.sublimetext.com/>`_
* `Atom <https://atom.io/>`_
* `PyCharm <https://www.jetbrains.com/pycharm/>`_

Open Source/Libraries
----------
One of the great ideas that the computer science community supports is the idea of open source software/code. The sharing of code that anyone has developed has created a positive reinforcement cycle that allows more advanced applications to be created without everyone having to start from scratch. Computer languages have adopted the idea through the creating of software libraries. Libraries are code that some third party has made that can be used for your own purposes. One of the biggest strengths of Python is the extensive development of software libraries that allow programmers to use Python to do things like manage radios to machine learning. In fact, the autopilot software was created through open source code! We've listed a couple libraries that may be of interest to teams:

* `matplotlib <https://matplotlib.org/>`_
* `scipy <https://www.scipy.org/>`_
* `numpy <https://numpy.org/>`_
* `dronekit <https://dronekit.io/>`_
* `arducopter <http://ardupilot.org/copter/>`_



Version Control
------
When you are writing code, saving often is a good way to make sure that your progress isn't lost. However, what if you decided to try something, but it didn't work out the way you had hoped to? Version control will allow you to revert back to not just what you saved previously, but every version that you saved! That way, you can go back to any version of code that you had previously. `Git <https://git-scm.com/>`_ (the computer version), `Github <https://github.com/>`_ ,  and `Gitlab <https://about.gitlab.com/>`_ (both web based versions) are primary examples of easy to use version control software. For help in setting version control up as well as a better introduction, https://try.github.io/ should help.

Debugging Tips
---------
Coming soon!



Best Practices
-------
1. Use version control: This will allow teams to manage their code and allow different people to work on different parts at the same time. 
2. Test often and early. Don't wait til you're "done" to test out your code! There may be some bug in the beginning that you will need to take care of that may affect the rest of the code! Find that bug early before moving on! 
3. Plan out your code structure beforehand. This will help save time and reduce errors as you move along coding.
4. Use comments! Document your code so that other people who read it can understand what you are trying to do.



Resources
*************
Below are some resources that should be helpful for teams to fully learn how to program

Intro
-------
* `Codeacademy <https://www.codecademy.com/>`_

* `Scratch <https://scratch.mit.edu/>`_

* `Learn Python <https://www.learnpython.org/>`_


Intermediate
--------
* `Dive into Python <https://diveintopython3.problemsolving.io/>`_

* `stack overflow <https://stackoverflow.com/>`_




Advanced
-----------
* `Introduction to Algorithms by Cormen <http://web.ist.utl.pt/~fabio.ferreira/material/asa/clrs.pdf>`_

* `MIT OCW <https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-00-introduction-to-computer-science-and-programming-fall-2008/>`_



2021-2022 Competition Specific Material
*****************

Example code for the competition can be found here: https://github.com/aeroroboticscomp/ARC-example. 

THe primary task for teams is to create a computer program that will allow teams to determine the optimal path to traverse the waypoints. In past years, we have asked teams to come up with a program that will compute the path, transfer the path to the drone, and then have the drone execute the mission. However, this year, we are only asking teams to compute the path. Therefore, teams should focus on designing a computer program to do so.

In the github link at the top, the 2021-2022 folder contains example codes as well as example mini-lessons on coding to help teams get started and understand how code can be written. All of these are made in Python; however, teams are NOT required to use Python. Any non-GUI based programming language would suffice (ex. C, C++, Java, Perl, FORTRAN, etc.) . 

NOTE: For Python users, Jupyter notebooks and equivalents are allowed. Please email ARC Staff if you have any questions. 

To help with getting started on the tasks and learning, please see the Mini-Lessons page that has been created. 
