# Paper Puppets

*A lab report by Zwee Dao*

## In this Report

To submit your lab, clone [this repository](https://github.com/FAR-Lab/IDD-Fa18-Lab4). You'll need to describe your design, include a video of your paper display in operation, and upload any code you wrote to make it move.

## Part A. Actuating DC motors

**Link to a video of your virbation motor**

[Vibrator video](/vibrator.MOV)

## Part B. Actuating Servo motors

### Part 1. Connect the Servo to your breadboard

**a. Which color wires correspond to power, ground and signal?**
Red - power
Brown - ground
Yellow - signal

### Part 2. Connect the Servo to your Arduino

**a. Which Arduino pin should the signal line of the servo be attached to?**
pin 9

**b. What aspects of the Servo code control angle or speed?**
This code which uses `myservo.write()` to set servo position:

<pre><code>
for(pos = 0; pos <= 180; pos += 1) // goes from 0 degrees to 180 degrees
  {                                  // in steps of 1 degree
    myservo.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);                       // waits 15ms for the servo to reach the position
  }
  for(pos = 180; pos>=0; pos-=1)     // goes from 180 degrees to 0 degrees
  {
    myservo.write(pos);              // tell servo to go to position in variable 'pos'
    delay(15);                       // waits 15ms for the servo to reach the position
  }
</code></pre>

## Part C. Integrating input and output

**Include a photo/movie of your raw circuit in action.**

[Potential meter & servo video](/servo.MOV)

## Part D. Paper puppet

**a. Make a video of your proto puppet.**

[Puppet video](/puppet.MOV)

## Part E. Make it your own

**a. Make a video of your final design.**

[Puppet video](/puppet.MOV)
 
