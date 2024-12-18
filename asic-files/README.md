# Wristwatch Controller ASIC
## CSE 30342 - Digital Integrated Circuits - University of Notre Dame

### Group Members

- Gabe Hinrichs (ghinrich@nd.edu)
- Ben Walsh (bwalsh7@nd.edu)
- AJ Sullivan (asulli27@nd.edu)
- Will Stotz (wstotz@nd.edu)

### Project Description

We have created an ASIC chip that implements the functionality of a 24-hour wristwatch with an alarm. Users can set the time to any hour and minute. The seconds place can be zeroed like a normal consumer watch. They can also set any hour and minute to be the desired alarm time. Once that time is reached, the alarm will remain active until cleared. The watch outputs to a conventional, addressable, four-digit seven-segment display, a photo of the external circuit is attached. The time is kept by a 32kHz oscillator and a counter ticking up at each clock signal and adding a second every 32,768 ticks.

The included test bench sets the alarm to 00:02 and the time to 23:51. During the minute 23:54 the seconds are zeroed making that minute appear noticably longer. All digits are displayed including the rollover from 23:59 to 00:00. The alarm triggers at 00:02 and is reset about a minute later.