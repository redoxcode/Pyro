# Building instructions
![image](images/build_1.jpg)
## 1. Before you start
- Before you start with any step, make sure to read all the text for that step.
- If you don't have that much soldering experience we recomment you read this [excellent guide](https://learn.adafruit.com/adafruit-guide-excellent-soldering).
- We found it easiest and got the best results by doing things in this order.
- You might be able to skip some steps depending on your kit / parts.
- To get a clean build a lot of dry fitting should be used. That means you loosely stack all the parts needed and once everything is in place you start to solder. Sometimes you can use a small tape or rubber band to keep everything together. Start by soldering 2 opposing pins per component to keep everything in place. Then solder all the other pins.
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
- Your display should already have some male headers

![image](images/cut_headers.jpg)
## 3. Separate the front and the back PCB
- Use the diagonal cutters with the flat side facing the PCB and the angled facing the bridge.
- Cleanup the edges if needed.

![image](images/cut_pcb.jpg)
## 4. Select the display pinout
- There are 2 solder jumpers (J1 and J2) on the back of the front PCB. These are used to select the display layout. You have to connect the center pad with the right OR with the left pad.
- Compare your displays pin layout to the one printed on the front PCB.
- If they match:
  - For both jumpers: Connect the center pad to the pad WITH the '^' marking
- If Gnd and Vcc are swapped:
  - For both jumpers: Connect the center pad to the pad WITHOUT the '^' marking
- Use the multimeter to check that there is no connection between Gnd and Vcc of the display header.
- If you have a connection between these points, one of the jumpers is causing a short circuit.

![image](images/build_8.jpg)
## 5. Solder headers between the PCBs
- The PCBs are connected by 3 headers that are 8 pins long each.
- Dry fit everything first and once everything is in place start to solder the whole assembly!
- The headers should be on the same side of the PCBs as the smileys. So the smileys should face each other in the final assembly!
- The male headers should be soldered to the main PCB (the one with the Pyro logo). The female headers should be soldered to the front PCB (the one with the jack sockets).

![image](images/build_2.jpg)
## 6. Check the ground (Gnd) connection
- Use a multimeter to check that both PCBs have a good ground (Gnd) connection. Measure the resistance between the 'Gnd' pin of the 'I2C EX' header on the main PCB) and the negative (-) pin of 'LED1' on the front PCB. The resistance should be 1 Ohm or less.
- If it is more:
  - Check that your multimeter shows 0 Ohm if you connect both probes directly.
  - Check all solder joints of the headers.
- If everything is good, separate both PCBs again and continue.

![image](images/build_3.jpg)
## 7. Solder the eurorack power connector
- Solder the male 10-pin IDC connector for the eurorack power cable.
- The eurorack power connector is located left of the Pyro logo on the main PCB.
- The 'I2C EX' header should only be soldered if you need it to connect extension modules.

## 8. Solder male headers to the RP2040 board
- Use a breadboard to make sure the headers are straight.
- The 4 pin header is not used and should not be soldered.
- Be carefull to not bend any pins when you remove the assembly from the breadboard.

![image](images/rp2040_board.jpg)
## 9. Solder female headers for the RP2040 board
- Dry fit the RP2040 board with the female headers onto the main PCB.
- The RP2040 board should be on the same side as the Pyro logo.
- Once everything is in place start to solder.

![image](images/build_5.jpg)
## 10. install the display
- Use the small distance pieces and screws (M2.5) to mount the display.
- The display header will be barely long enouth. So you might have to solder between the display and the PCB. Just make sure there is a good connection.

![image](images/build_7.jpg)
## 11. Dry fit and solder the jack sockets
- Dry fit the jack sockets together with the front panel to the front PCB.
- Once everything is in place start to solder.

![image](images/build_9.jpg)
## 12. Dry fit and solder the encoders
- Dry fit the encoders together with the front panel to the front PCB.
- Screwing the hex nuts a few rotations onto the encoders will help getting them straight.
- Once everything is in place solder just the 2 large pins to keep them in place.
- If you are happy with the encoders position solder the other 5 pins.

![image](images/build_10.jpg)
## 13. Dry fit and solder the LEDs
- Attantion: You might have 6 LEDs of one color (Output 1 to 6) and 2 LEDs of a different color (Output A and B)!
- Make sure to get the polarity right (longer leg of the LED is +)!
- Dry fit the LEDs together with the front panel to the front PCB.
- Once everything is in place start to solder.

![image](images/build_11.jpg)
## 14. Final assembly
- Assemble the main PCB with the RP2040 board to the front PCB and panel.
- Add Knobs to the encoders. make sure they are easy to turn and press (they should shound klicky when pressed down).

![image](images/build_12.jpg)
