# csc-355-lab-7-finite-state-machine-design-solved
**TO GET THIS SOLUTION VISIT:** [CSC 355 Lab 7: Finite State Machine Design Solved](https://www.ankitcodinghub.com/product/csc-355-lab-7-finite-state-machine-design-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;7742&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSC 355 Lab 7: Finite State Machine Design Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Introduction

This lab provides practice designing and (possibly) implementing a Finite State Machine (FSM) starting either from some initial specifications of the problem to be solved or from a given State Diagram.

Pre-Lab Exercises

1. Pre-Lab #1 : FSM #1

You are part of a design team that has been asked to design a controller for a home heating system to be marketed across the cold Canadian prairies.1 Heat is provided from two sources, a natural gas fired furnace and a passive solar window system that includes insulated shutters. If the sun is shining2 and the outdoor temperature is more that -25o C the windows provide enough heat to warm the building. When there are clouds in the sky, when it is very cold (≤-25o C) and during the night the windows shed heat and the shutters must be closed.

The specification of the controller is as follows:

There are three external inputs (simulated using data switches):

 D, which is to be attached to a solar detector. However, in the laboratory testing environment, a simple data switch is used to simulate the input from this device. Hence D set to 1 indicates that the sun is shining and a 0 indicates that it is not.

 T, which is to be attached to a thermostat placed inside the house. It returns a 1 when the building needs more heat and a 0 when it does not.

 G, which is attached to an outdoor temperature sensor. It returns a 1 when the outdoor temperature is &gt; -25o C, and a 0 otherwise.

The controller can be in four different states:

 S0: In this state the furnace (F) is off and the shutters (S) are closed. Thus state S0 is labeled with two bit state variables, F = 0 and S = 0.

 S1: In this state the furnace is on and the shutters are open. Thus state S1 is labeled with two bit state variables, F = 1 and S = 1.

 S2: In this state the furnace is on and the shutters are closed. Thus state S2 is labeled with two bit state variables, F = 1 and S = 0.

 S3: In this state the furnace is off and the shutters are open. Thus state S3 is labeled with two bit state variables, F = 0 and S = 1.

1 In this climate it is very cold for half the year and every home must be heated.

2 Fortunately the sun shines frequently.

Lab 7: Finite State Machine Design

CSC 355 Last update October 2016 Page 2 of 8

The table below indicates the results of the analysis phase of this project.

From state

Input sensors: DTG=

Go to state:

S0

000, 001, 100 or 101

S0

110

S1

010 or 011

S2

111

S3

S1

000, 001, 100 or 101

S0

110

S1

010, 011 or 111

S2

S2

000, 001, 100 or 101

S0

110

S1

010 or 011

S2

111

S3

S3

000, 001, 100 or 101

S0

110

S1

010 or 011

S2

111

S3

All other input combinations cause the system to go to state S3. The sequential machine for the controller has four states and uses two state variables for this purpose, F and S. F and S can be monitored using two output LEDs

a) Draw the state diagram for a FSM to represent the given specifications above.

b) Write an encoded state table (transition table) corresponding to the state diagram of the previous step.

c) Fill in the Karnaugh maps for the next states F+, S+, and write minimal sum-of-products equations for F+, S+ (show your work).

d) For the circuit, it has been decided to use D flip-flops, so the equations created in c) above can be used directly for the flip-flow inputs. (i.e., D=Q+). On a separate piece of paper that you bring with you to your lab, draw the complete circuit diagram (properly labeled), including pin numbers, for your design.

Note: A maximum of one 7474, three 7400, one 7404 and one 7410 chips can be used!

2. Pre-Lab #2: FSM #2

Design a circuit with the specifications described below.

 External inputs: A, B, C and D, controlled from the data switches.

 Number of states: 4 (The state assignment to be used is defined below.)

 Outputs: Two LEDs to monitor the values of the state variables, called X and Y.

 State diagram: shown here:

A+B

_ _

C D

_ _

A C

A C

B C

_ _

A B

S0

S3

S2

S1

____

B + C

_ _

B C + B C

Lab 7: Finite State Machine Design

CSC 355 Last update October 2016 Page 3 of 8

a) Complete a state table corresponding to the state diagram. Use don’t cares for input combinations, where appropriate, so that your table can be abbreviated. In the example on the pre-lab worksheet, the first four rows are shown as a guide. Make sure that the total number of rows (i.e., combinations for A, B, C and D) covers all the 16 possibilities for each of the states. (You may not need all of the rows shown in the table.)

b) Complete the encoded state table (transition table) corresponding to the state table of the previous step. Use the following state assignment (it will be just the first and last columns that change – the number of rows you use will be the same as in the previous part):

State

X

Y

S0

0

0

S1

0

1

S2

1

0

S3

1

1

c) Fill in the Karnaugh maps for the next states X+, Y+. Remember that X+ and Y+ are functions of X, Y, A, B, C and D. Please use this ordering of inputs.

d) From these maps, fill in the maps for the inputs for J-K flip flops representing X and Y. You need 4 Karnaugh maps of 6 inputs each.

e) Determine the minimal sum-of-products equations for each of JX, KX, JY and KY.

f) On a separate piece of paper that you bring with you to your lab, draw the complete circuit diagram (properly labeled), including pin numbers, for your complete circuit design.

Note: A maximum of three 7400 chips, one 7404 chip, one 7410 chip and one 7476 chip can be used for this experiment.

Part 2: Procedures for the In-Lab Exercises

1. Greet your lab instructor and obtain your graded Pre-Lab 7.

2. Build circuit 1 and demo its functions to the lab instructor.

3. Build circuit 2 and demo its functions to the lab instructor.

Lab 7: Finite State Machine Design

CSC 355 Last update October 2016 Page 4 of 8

Pre-Lab Worksheet #7 NAME: _________________ LAB Section: B0__

1 a) Draw the state diagram for a FSM to represent the given specifications.

1 b) Write an encoded state table (transition table) corresponding to the state diagram above.

Present

State

Next

State

F+ S+

F

S

DTG = 000

DTG = 001

DTG = 010

DTG = 011

DTG = 100

DTG = 101

DTG = 110

DTG = 111

0

0

0

1

1

0

1

1

1 c) Fill in the Karnaugh maps and write minimal sum-of-products equations

FS\TG

00

01

11

10

FS\TG

00

01

11

10

00

00

01

01

11

11

10

10

D=0

D=1

F + =

FS\TG

00

01

11

10

FS\TG

00

01

11

10

00

00

01

01

11

11

10

10

D=0

D=1

S + =

Lab 7: Finite State Machine Design

CSC 355 Last update October 2016 Page 5 of 8

2 a) Complete a state table corresponding to the state diagram.

present state

condition

next state

A

B

C

D

S0

0

0

x

x

S0

S0

1

x

x

x

S1

S0

x

1

x

x

S1

S1

x

x

0

0

S2

2 b) Complete the encoded state table (transition table).

present state

condition

next state

XY

A

B

C

D

X+Y+

00

0

0

x

x

0 0

00

1

x

x

x

0 1

00

x

1

x

x

0 1

01

x

x

0

0

1 0

Lab 7: Finite State Machine Design

CSC 355 Last update October 2016 Page 6 of 8

2 c) Fill in the Karnaugh maps for the next states X+, Y+.

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=00

XY=01

Maps for X+

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=10

XY=11

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=00

XY=01

Maps for Y+

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=10

XY=11

Lab 7: Finite State Machine Design

CSC 355 Last update October 2016 Page 7 of 8

2 d) Fill in the maps for each of JX, KX, JY and KY.

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=00

XY=01

Map for JX

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=10

XY=11

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=00

XY=01

Map for KX

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=10

XY=11

Lab 7: Finite State Machine Design

CSC 355 Last update October 2016 Page 8 of 8

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=00

XY=01

Map for JY

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=10

XY=11

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=00

XY=01

Map for KY

AB\CD

00

01

11

10

AB\CD

00

01

11

10

00

00

01

01

11

11

10

10

XY=10

XY=11

2 e) Determine the minimal sum-of-products equations for each of JX, KX, JY and KY.

JX= KX =

JY = KY.=
