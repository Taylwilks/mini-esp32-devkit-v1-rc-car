⚠️ Important Notes
-
Soldering Required:

This build involves soldering, including directly to the ESP32 board. If you're not comfortable with soldering A jumper cable-compatible version may be released in the future.

Frame Version Recommendation: 

Print only Frame v3 or higher for optimal results. Earlier versions may be fragile or require additional adjustments.

🛠️ Materials Needed

.1x ESP32 Devkit V1

.2x N20 Motors

.1x DRV8833 Motor Driver Board (I recommend the smaller black version)

.1x Li-ion Battery (Rechargeable preferred)

.M2 Screws (Various sizes)

.JST Connectors

.Micro USB or USB-C Cable (Depending on your ESP32 board)

.Double-Sided Tape (Or fold regular tape over itself)

.Stranded Core Insulated Wire (Various lengths)

.hot glue or super glue


🖨️ Step 1: Print the Frame
-
Download the provided STL files or click this link to take you to the maker world site    ( link coming soon ).

Note: Earlier frame versions (v1 and v2) are experimental and may not perform well.
Use Frame v3 or above for the best durability and fit.
Print the files using your preferred 3D printer.

🔌 Step 2: Flash the Firmware
-
Download the firmware (currently under development).
Use the Arduino IDE (or another tool compatible with ESP32) to upload the code.
Firmware status: Not yet available (expected soon).
Updates and troubleshooting will be added once the firmware is ready.

🛠️ Step 3: Assemble the Components
-
.1: first of all you will need to remove the suports from the print ( if you can print it to need less suports good on you )

.2: solder the out+ and out- of the tp4056 to the in+ and in- of the boost converter 

.3: place the battery in the space under the esp32 slot feeding the two leads under the esp32 slot ( make sure the two exposed parts of the leads leads dont touch )

.4: solder the + and - wires of the battery to the respective pads on the tp4056 labeld B+ and B- ensuring to first cut the red wire in half soldering a slide switch inbetween both halfes

.5: using a multimeater and a small screw driver set the boost converter to a steady 5v

.6: eather glue ore tape the two boards to the undeside of the frame 

.7: solder two leads to each of the motors exposed pins (to make your life easier use two distinked colors) giving one motor wires about 2cm long and the other about 6cm long

.8: connect the other end of the wires to the drv8833 (make sure to group the motor wires E.G. motor 1 - out 1 - 2)

.9: from the boost converter run two leads (red and black) from the out + and - pads to the gnd and vcc pins on the drv8833 and to the vin and gnd pins on the esp32 board

.10: on the back of the drv8833 there are pins labeld in 1 - 4, run a wire from each one to the data pins D23 D22 D21 and D19 respectivly 

.11: fit the motor wheels on the motor rod x2 and the non motor wheels in the empty wheel sockets (the non motor wheels will need 1 screw each

.12: conect the esp32 to you computer and using arduino idle flash the provided firmware to the esp32 

.13: now get your duleshock 4 controler and hold down the share and PS button until the light flashes then waight for it to connect to the esp32

.14: now we can test, when you press X the car should move forward, triangle backwards, and the left and right arrows will move left and right respectivlty
        (if the motors move the wrong way you will need to swap the motor wires around.

.15: cause mayhem with your new rc esp32 car

💡 Tips and Future Updates
-
A jumper cable-compatible version may be avalible sometime in the future for those who want a solder-free experience.
Check back for firmware updates and enhanced frame designs.

🤝 Contributions and Support
-
If you have ideas, find bugs, or want to improve this project, feel free to open an issue or submit a pull request.
