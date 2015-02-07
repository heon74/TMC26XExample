# TMC26XExample
The TOS-100 is an Arduino compatible shield capable of driving one bipolar stepper motor up to 1.7A that utilizes the Trinamic Motion Control TMC260 stepper motor driver chip.

http://www.motioncontrol-community.org/?page_id=36#tos100

---

The code is currently compiling error free, but there are issues with the constructor definition before thee setup() in the .ino file.

If flashing the code as is, it puts the Core in a white flashing mode.

Putting the constructur inside the setup(), removes the Core mode of flahsing white, but then the construtor is no longer Global.

I have made changes to the following lines, in the original files from http://www.motioncontrol-community.org/?page_id=36#tos100

.ino: row 25

.cpp: row 28, 36, 172, 379, 962

.h: no changes

The changes are expolained in the code.
