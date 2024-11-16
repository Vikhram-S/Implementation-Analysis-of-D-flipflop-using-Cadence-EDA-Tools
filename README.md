# Implementation-Analysis-of-D-flipflop-using-Cadence-EDA-Tools
Ex No: 01     Implementation & Analysis of D-flipflop using Cadence EDA Tools   

Aim:
To design and implement a D-flip-flop using Cadence EDA tools, simulate its behavior, and analyze key perfoacrmance parameters such as timing, power consumption, and resource utilization for a comprehensive understanding of sequential logic circuits.

Tools Required:
•	Personal Computer
•	Cadence Virtuoso Software

Circuit Diagram:

![IMG-20241115-WA0005](https://github.com/user-attachments/assets/65ea86c2-ccb3-4f94-b2ec-035f42896902)



S C H E M A T I C S I M U L A T I O N - PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION -Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
•	csh
•	source /cadence/install/cshrc
•	virtuoso 
Procedure for Schematic simulation using Cadence

1.	Now two windows must open i) virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.
i.	Create a New Library
ii.	Create Schematic Cell view.
iii.	Create the Symbol for schematic Cell view.
iv.	Create the test Cell view.
v.	Analog simulation by spectre


i)	Procedure for Creating New Library.
•	File –New – Library
•	Name: Give name for ur library Ex: VLSILAB_EXP_1
•	Enable Attach to an existing technology library, Click OK
•	Attach the library to the technology library gpdk045.Click OK
ii)	Create Schematic Cell view.
•	Go to 1st window i.e virtuoso (CIW)
•	File-New-Cell view
•	Setup the new file form
	Library: Select the one you created.
	Cell: Give the experiment name Ex: Inverter ViewSchematic
	Type: Schematic press OK
•	Add the required components from the libraries and make the connections.
	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	Click on browse. This opens the library browser
	Now select the appropriate library for components like 
	Gpdk45 ------------------------nmos1v, pmos1v
	Create Input and Output pins
	Make the connections by using fixed narrow wire key
	Click Check and Save button
![Screenshot 2024-10-21 183932](https://github.com/user-attachments/assets/aa5a1ae8-d448-42ae-abe9-206b3c2d91e9)




 
iii)	Creating the Symbol for schematic Cell view

•	In the schematic window, execute 
	Create – Cell view – From Cell view
	The cell view from cell view window appears
	Check Lib Name, Cell Name, From View name must be schematic Press ok
•	Now Symbol generation form appears. Click Ok If No changes required
•	A new window with with default symbol is created.
•	Edit the symbol if you want to give actual symbol shape else continue.
•	Execute Create-Cell view-from cell view
•	Library Name and Cell Name must be same which you have used for schematic. Press OK
•	Check for the position of pin side.Prss OK
•	Edit for the shape by Create-Shape-Choose required options to edit.
![Screenshot 2024-10-21 184322](https://github.com/user-attachments/assets/7e57d9c0-ec1c-47ed-a24d-207686f31bda)



iv)	Creating the new test cell view

•	Go to CIW window, Execute File-New-Cell view
	Setup the new file form
	Library: Select the one you created.
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	View: Schematic
	Type: Schematic press OK
•	Follow the step 3(ii) d to make the required connections

![Screenshot 2024-10-21 185248](https://github.com/user-attachments/assets/7c652d51-59f0-4ca4-b63d-c40ac73c1454)



 
Analog simulation by SPECTRE.
•	In test cell view window
•	Launch – ADE L(Analog Design Environment)
	Execute Setup—Simulation/directory/Host A new window opens
	Set the simulation window to spectre and click ok
	Execute Analysis – Choose. A window opens.
	Select the type and set the specifications and press OK
	Execute Output s—to be plotted – Select on Schematic
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
•	Execute Simulation -- Net list and Run
 
![Screenshot 2024-10-21 192323](https://github.com/user-attachments/assets/9a54381d-3da1-461c-910b-d2181612cbee)



For Transient Analysis Settings 
 
![Screenshot 2024-10-21 185609](https://github.com/user-attachments/assets/6d3d5199-bec0-4d64-b9fd-cbf55e6a92c5)

 Output
 ![Screenshot 2024-10-21 192517](https://github.com/user-attachments/assets/595cee10-081e-49d8-af5c-923645123372)



Results:
The design and implementation of the D-flip-flop using Cadence EDA tools were successfully completed. The simulated results confirmed the correct operation of the flip-flop, with proper synchronization of the input data with the clock signal. Key performance parameters such as propagation delay, power consumption, and area utilization were evaluated, aligning with expected theoretical values.











