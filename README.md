# LogicGates_IC_layout


Repository of Schematic diagram , VLSI layout , simulation graph of Logic gates and IC 

> Basically I am using Electric VLSI design system to design Logic gates and IC's schematic diagram and layouts. <br>
> I always simulate all the things in LTSpice XVII software to get or check the output is correct or not.

<pre>  </pre>
  <a href="https://en.wikipedia.org/wiki/Electric_(software)" target="_blank">
    <img src="https://www.gnu.org/software/electric/electric.jpg" alt="electric VLSI" width="40" height="40"/>
  </a>
  Electric VLSI Design System
  <br><br>
 <a href="https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html" target="_blank">
   <img src="https://ez.analog.com/cfs-file/__key/communityserver-components-groupavatars/00-00-00-06-51/LTspice_2D00_Icon.png_2D00_320x240.png.png" alt="electric VLSI" width="40" height="40"/>
</a>
  LTSpice XVII
  <br><br>
  
> N.B : Make sure that you have installed Jdk first. Electric VLSI needs java run time Environment to operate.


I will update this repository as soon as possible.
## Here is basic info about this gates and ICs

<div align="center">
  
# NOR Gate
  
</div>

<br>
  The NOR gate represents the complement of the OR operation. The NOR gate is also a universal gate,combination of the NOT-OR gate.<br>
  The logical or Boolean expression for the NOR gate is --
  
<div align="center">
   Y= (A + B)'
<div>
    
### Symbol
    
<img src="https://upload.wikimedia.org/wikipedia/commons/1/15/Logic-gate-nor-us.png" alt="symbol" width="300px" height="150px"><br><br>
<img src="https://concept-stories.s3.ap-south-1.amazonaws.com/test/Stories%20-%20Images_story_50534/image_2019-06-19%2017%3A41%3A30.765401%2B00%3A00">
  
  
 Design with CMOS transistor
  
  <img src="https://eepower.com/uploads/articles/basic-cmos-logic-gates-fig3.jpg">
  
### Truth Table
  
  <img src="https://static.javatpoint.com/tutorial/digital-electronics/images/nor-gate-in-digital-electronics3.png" alt="truth_table"><br><br>
  
  
If you want to know further about NOR gate [click here](https://en.wikipedia.org/wiki/NOR_gate)
  
<div align="left">
  
## Here's the screenshot of my projects
  
</div>
  
  
<img src="https://raw.githubusercontent.com/AmitBarman99/LogicGates_IC_layout/master/NOR_gate/Screenshot%20(11).png" alt="Nor_layout_vlsi">
  
layout design of NOR gate (Electric vlsi)
  
<br>
<img src="https://raw.githubusercontent.com/AmitBarman99/LogicGates_IC_layout/master/NOR_gate/Screenshot%20(3).png" alt="Nor_simulation">
  
Simulation of NOR gate (LTSpice XVII)
  
<div align="left">
  
# Important


During this Simulation you need to provide input signal or spice code
this code is here,
  
  ```bash
  vdd vdd 0 DC 5
va A 0 DC pwl 10n 0 20n 5 50n 5 60n 0 90n 0 100n 5 130n 5 140n 0 170n 0 180n 5
vb B 0 DC pwl 10n 0 20n 5 100n 5 110n 0
.measure tran tf trig v(AnorB) val=4.5 fall=1 td=4ns trag v(AnorB) val=0.5 fall=1
.measure tran tr trig v(AnorB) val=0.5 rise=1 td=4ns trag v(AnorB) val=4.5 rise=1
.tran 200n
.include D:\Electric\projects\C5_models.txt
  ```
 
  
> If you will face any type of problems, feel free to ask <br>
> And <br>
> Be aware from layout shorts and DRC-ERC errors.😁
  
## All the best
  
</div>
