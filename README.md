# DC_Motor_Control_System
A DC motor control system to control a 180VDC motor for applications in machinery modifications.

Keypad_MCP23008_I2C_Module This new project is to continue with making a stand alone I2C matrix keypad for future projects. My main hobby is building my own workshop equipment or restoring equipment I find abandoned. I am currently working on a bench top milling machine and a small hobby lathe. Both of these need new motors. I have opted to using reclaimed treadmill motors (180VDC, 4700RPM, 2-2.5HP). To use these motors I need to build a H-Bridge controller and the user interface. DC controllers to meet the motor specifications are almost impossible to get in Australia and would be very expensive. This project is specifically about building the User Interface.

The interface will consist of:

16 key 4x4 matrix keypad (heavy duty) 16x2 LCD display with I2C backpack MCP23008 I2C I/O expander I/C case (custom built) start button (to start motor) - example only model may change on availability stop button (to stop motor) - example only model may change on availability Arduino Uno or stand alone ATMEL328P circuit Project Scope:

Provide a means of entering desired RPMs or Feed rates (mm/min) Display entered values and user information Output key data to microcontroller Start/Stop functions Microcontroller functions concatenate individual characters into an array and convert to an integer map integer to PWM value and store as: one off speed preset speed values output PWM values to H-Bridge controller monitor motor RPM and current and store values from sensor readings manage PID feedback.
