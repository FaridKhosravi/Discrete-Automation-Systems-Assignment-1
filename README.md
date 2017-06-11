# Discrete-Automation-Systems-Assignment-1

Objective:
The first assignment objective is to develop a basic PLC program using Beckhoff TwinCAT (So, also getting to know the tool).

Any approach you could imagine can be used for the program development. The main criteria for the evaluation is the working program. 

Task - System to develop:
The system is composed of a conveyor and a tank. The conveyor is used to deliver empty containers under the tank. The container should stop under the tank to get filled. Once filled, the container is transported out of the system. The tank has capacity to fill in 10 containers, after which system should stop until the tank is refiled to serve new containers.

Outputs:
1)Motor - the motor to control the conveyor.
2)Valve - to open for filling in the container.
3)Tank_empty_out - the led to signal that the tank got empty.


Inputs: 
1)Container_in_place - the container is under the tank in the filling position (probably a good moment to stop the conveyor for filling up the container).
2)Container_full - sensor telling when the container is full (probably the good way to decide when the valve of the tank should be opened/closed).
3)Tank_empty_in - sensor telling when the tank is empty (probably a good moment to signal with the led (Tank_empty_out) the operator about the situation).
4)Loading - just a button to signal the input of the container.
5)Unloading - just a button to signal the removal of the container from the system.
6)START - a button to tell system to run.
7)STOP - a button to stop the system.
8)EMERGENCY - a button to give an emergency signal (system should get into the safety mode: valve closed, motor turned off).
