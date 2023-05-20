Transfer Function Analysis

This Python code analyzes the behavior of a given transfer function. It performs various analyses and generates corresponding plots to provide insights into the system's dynamics and stability.

Prerequisites

numpy library
matplotlib library
scipy library
Make sure these libraries are installed in your Python environment before running the code.

Description

The code analyzes the transfer function with coefficients num and den, representing a second-order system. The transfer function is created using the TransferFunction class from the scipy.signal module.

The following analyses are performed:

Impulse response analysis:
The impulse response of the transfer function is computed using signal.impulse.
The resulting time and output values are stored in t_imp and y_imp, respectively.
An impulse response plot is generated to visualize the system's response to an impulse input.
Step response analysis:
The step response of the transfer function is computed using signal.step.
The resulting time and output values are stored in t_step and y_step, respectively.
A step response plot is generated to visualize the system's response to a step input.
Frequency response analysis:
The frequency response of the transfer function is computed using signal.bode.
The resulting frequency, magnitude, and phase values are stored in w, mag, and phase, respectively.
A magnitude response plot is generated to visualize the system's gain across different frequencies.
Stability analysis:
The stability of the system is determined by checking the location of the transfer function's poles.
The code calculates the roots of the denominator polynomial using np.roots(den) and checks if all the real parts are negative.
The stability analysis result is printed, indicating whether the system is stable or unstable.
Usage
Ensure that the required libraries (numpy, matplotlib, and scipy) are installed.
Set the coefficients of the transfer function (num and den) according to your specific system.
Run the code. The plots will be displayed, and the stability analysis result will be printed.
