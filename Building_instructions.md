# Building instructions
## 1. Before you start
- If you don't have that much soldering experience we recomment you read this [excellent guide](https://learn.adafruit.com/adafruit-guide-excellent-soldering).
- You might be able to skip some steps depending on your Kit / Parts.
- Your PCBs might look slightly different than those in the pictures.
## 2. Prepare your headers
- You might need to cut your headers to the right length.
- You need:
  - 2 male and 2 female headers for the RP2040 board (20 pins long)
  - 3 male and 3 female headers 8 pins long
- To separate male headers: 
  - Grab the pins before and after the point of separation and twist them.
- To separate female headers: 
  - Use the diagonal cutters and cut in the middle of the next socket (you will have to sacrifice one socket).
  - Make sure the flat side is facing the part of the header strip you want to use.
  - Cleanup the edges if needed.
## 3. Solder male headers to the RP2040 board
- Use a breadboard to make sure the headers are straight. 
- Be carefull to not bend any pins when you remove the assembly from the breadboard.
![image](images/rp2040_board.jpg)
## 4. Separate the front and the back PCB
- Use the diagonal cutters with the flat side facing the PCB and the angled facing the bridge.
- Cleanup the edges if needed.
![image](images/cut_pcb.jpg)
## 5. Solder headers between the PCBs
- The PCBs are connected by 3 headers that are 8 pins long each.
- Dry fit everything first and once everything is in place start to solder the whole assembly!
- Both PCBs have a smiley printed on them. These smileys should face each other in the final assembly!
- The male headers should be soldered to the main PCB (the one with the Pyro logo).
- The female headers should be soldered to the front PCB (the one with the jack sockets).
