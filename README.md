# arduino-oled-display
Code and instructions to build a customizable OLED display animation with Arduino Nano. 
Perfect as a creative project, gift, or exciting decoration. 

NOTE: Some code taken from Tigris Li (https://github.com/tigrisli). This new code makes use of GIMP to convert animations into bitmaps instead of using Processing.

# Materials Used
- 0.96" OLED Module (I²C, White) - $9.99 CAD Canada Robotix
- Elegoo UNO R3 w/ included ethernet cable - $23.99 CAD Amazon
- Elegoo Small Breadboard - $10.99 CAD - Amazon
- 4 Jumper Wires - $12.27 CAD Amazon
- Arduino (Nano) 

# Building 
  1. Connect the following pins to one another, from OLED display to ARDUINO:
     
     GND >> GND
     
     VCC >> 3V

     SCL >> SCL

     SDA >> SDA

     If using an Arduino without SCL and SDA, such as an Arduino Nano, we must utilize the Wire library.
     For this, connect:
     
     SCL > A5
     
     SDA > A4

  3. Similarly to Tigris' process, select a gif animation, resize, and split the frames
     
     Tips for choosing a gif:
     - Try not to choose an animation with too many frames as an Arduino may not be able to store all the information.
     - Choose an animation that only uses two tones (black and white), as shading is unlikely to work with an oled screen.
    
     RESIZE: https://ezgif.com/resize
     
     SPLIT: https://ezgif.com/split 


