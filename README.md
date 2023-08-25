### Control_of_buck_boost_converter
___

## Introduction
___

The output voltage in a power electronics converter can vary with a change in input voltage change in the load or changes in the duty cycle of the switching device. 
To obtain a constant output voltage, a controller is of the utmost importance. In many practical areas like PV solar plant input voltage varies significantly, this in turn will also make the output dc voltage, which is very much undesirable.
## Software Required
Install MATLAB software from here https://in.mathworks.com/products/matlab.html
Also, make sure to include the Simscape Electricals toolbox while installing Matlab software.

## Design of PID and Instruction
___

Vo = (D*Vin)/(1-D);

where Vo=Output voltage, D=duty cycle, Vin=Input Voltage.

In a buck-boost converter, we can change the output voltage by varying the converter's duty cycle.
This concept is employed in the PID controller design of the buck-boost converter.
Here in this project, I have assumed the reference voltage to be -13v.
You can change the reference voltage by double-clicking on the V_ref block of the Buck_boost_with_PID_controller.slx
A buck-boost converter without PID controller tuning is provided in Buck_Boost_converter_without_controller.slx.
The parameter are provided.
To tune the PID controller, double-click the PID block of the Buck_boost_PID.slx file.
Click the tune button inside the PID dialogue box.
## Reference 
___
https://www.saranathan.ac.in/emagazine/eee/sj/vol1_1/sjeee9.pdf
https://in.mathworks.com/help/slcontrol/gs/automated-tuning-of-simulink-pid-controller-block.html
