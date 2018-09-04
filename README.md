# IDD-Fa18-Lab1: Blink!

**A lab report by John Q. Student**

**Fork** this repository to get a template for Lab 1 for *Developing and Designing Interactive Devices* at Cornell Tech, Fall 2018. You should modify this `README.md` file to delete this paragraph and update below. As the lab asks:

> Include your responses to the bold questions on your own fork of the lab activities. Include snippets of code that explain what you did. Deliverables are due next Tuesday. Post your lab reports as `README.md` pages on your GitHub, and post a link to that on your main class hub page.

We've copied the questions from the lab here. Answer them below!

## Part A. Set Up a Breadboard

[insert a photo of your breadboard setup here]

![board](https://lh3.googleusercontent.com/QBVr_YLWR0opvDlymsypT3Rq8IWrAtjozOfyw7ZOPUhkioMUJznSfiylTjazM6Pkc2_eqFIaiZMxNzJOqTPqTe4s-H74DnSaG8amYWu0tu633f2E011S8ASJp3hRU57pcBhUS7PoNDI)


## Part B. Manually Blink a LED

**a. What color stripes are on a 100 Ohm resistor?**

Red, blue and purple.

![resistor](https://lh5.googleusercontent.com/QS92IlakxAEJdax2pe1ADKEEZkn0TDNPj26brwFzEXNfm3c1BpvSkSOW-Hhy8XRT1XUqqd9KDkf6u7e4XQHrDDAOjgdtdFDOvnsMxnvdJY8VNIKI_2qZHi8xp6236BYRzsZCCtBm9io)
 
**b. What do you have to do to light your LED?**

Connect the breadboard to the computer to power it up and make the whole circuit: resistor, button and LED.

## Part C. Blink a LED using Arduino

### 1. Blink the on-board LED

**a. What line(s) of code do you need to change to make the LED blink (like, at all)?**

Any, the function that came with the arduino blink function is set up to make blink the
built-in led which is in PIN 13.

**b. What line(s) of code do you need to change to change the rate of blinking?**

Need to change the delay.

```
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second
}
```

**c. What circuit element would you want to add to protect the board and external LED?**

A cable for ground.
 
**d. At what delay can you no longer *perceive* the LED blinking? How can you prove to yourself that it is, in fact, still blinking?**

I think it is between 10 and 15. 

### 2. Blink your LED

**Make a video of your LED blinking, and add it to your lab submission.**

[link to your video here; feel free to upload to youtube and just paste in a link here]

[video](https://drive.google.com/file/d/14yd1j7-7b5T6h-tKj72oH3EBcFKSmuV8/view?usp=sharing)


## Part D. Manually fade an LED

**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**


## Part E. Fade an LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**

I need to move the LED to one of the pins and place the resistance next to it.

**b. What is analogWrite()? How is that different than digitalWrite()?**

[video](https://drive.google.com/file/d/1KCOaEw5ekHULvaQjFxLA2mKFEii51FsB/view?usp=sharing)

## Part F. FRANKENLIGHT!!!

### 1. Take apart your electronic device, and draw a schematic of what is inside. 

**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**

**d. Is information stored in your device? Where? How?**

### 2. Using your schematic, figure out where a good point would be to hijack your device and implant an LED.

**Describe what you did here.**

### 3. Build your light!

**Make a video showing off your Frankenlight.**

**Include any schematics or photos in your lab write-up.**
