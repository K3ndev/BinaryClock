# Binary Clock

## Clock for programers

![my pcb](resurce/BinaryClock.png)

### Features

- Built in tiredness detector (if you cant read it you need to sleep)
- You can start conversations with it
- You can feel superior if you can read the time from it
- Displays the time in binary

### How can you make it?

1. Order the pcb (a stencil is recommended)
2. Order the parts from the bom
3. Print the holder
4. Solder in everything
5. Screw it up with 2 M2 screws
6. Plug the usb-c in
7. Set the time with the buttons
8. You got your Binary clock


### How it works

![draft schematic](resurce/image.png)

The crystals Hz is divided down to 1 Hz and it gives the circuit the clock.
T
here are some binary counter ic. The first one gets the clock straight from the crystal.

The others are getting from an AND gate with 4 input what is watching that the output of the pervious ic is don't flow over the limit. When all of the inputs are high it send a signal to de next ic's clock pin and the watched ic reset pin.
The counter pins are go straight to the leds trough a resistor.

There are 4 buttons. Those are for setting the time. Those buttons signal goes trough a low pass filter and a pulldown resistor to prevent multiple inputs in a same time. and the signals end at the ic's clock pin.

It's just a stand for the pcb
![Stand](resurce/render.png)

### License

This project is licensed under the MIT License - see the LICENSE file for details.