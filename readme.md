## Overview

So essentially this can be broken down into two guides. One on adding a USB-C port to your New 3DS XL and another on recovering a broken circlepad if things go wrong. If you just need to fix your circlepad, you can skip ahead to the troubleshooting section.

## Tools Needed
 - Soldering Iron (preferrably temp controlled but this is a rather simple mod so any will work)  
 - Wire (Black and red preferrably but any will work, I would recommend anything above 22 gauge, the smaller the better)  
 - USB-C Breakout Board (Sparkfun sells these otherwise Amazon does work, Amazon sells $4 on prime: https://a.co/d/fOM2OCB)
 - Fine files, and preferrably a rotary tool. The file is essential, rotary tool is recommended for starting.

## Main Guide

This is the most tedious process of the entire mod, it will take roughly half an hour to an hour depending. This is also the most important part cosmetically, if you mess up here there is no fixing it. So make sure you proceed carefully and have patience.

#### 1. Remove back panel.  
<img src="/images/IMG_0939.JPEG" alt="Back Cover" width="300" />
Remove the 8 screws, these are longer than the other screws in the console so be sure to keep them separate. The top two are covered by the rubber nubs, so also remove those and put them aside.

#### 2. Disconnect shoulder buttons
  These are connected via two small connectors, just lift up on these and they'll pop off.
  
#### 3. Drill and widen port
<img src="/images/IMG_0941.JPEG" alt="Finished port" width="300" />
The port should be roughly the same thickness of the holes for the carrying strap. Speaking of which, it's no longer usable with this mod. You cut the plastic to make it fit better. You also cute the plastic near the original charging port, this is to make the cables fit better as we will be bending them behind the mainboard.  

Filing the port is the most tedious part but it's all you will see on the outside, so take your time. A good hack is to try and fit the port outside the shell so you know the hole is the correct size. Basically just see if you can push it in from the outside. You also need to file down the stylus slot just a bit to make it seat better. When finished the port should fit like in the picture below.  

<img src="/images/IMG_0940.JPEG" alt="Finished mod" width="300" />

#### 4. Solder the port
This is not as hard as it seems. Basically we take the top right pin and solder it to VBUS or VCC on the usb-c port, use extra wire and cut to length when ready. Solder ground to the bottom right pin on the port, use extra wire and also cut to length when ready. Route the cables behind the motherboard by unscrewing the two top screws and flexing the PCB. This is my preferred method that doesn't harm other components (Will explain more in troubleshooting section). Once it's wired under the board, solder it to the correspond parts of the breakout board, thread the wires through the screw hole on the board. This is for cable management mainly.  
<img src="/images/IMG_0942.JPEG" alt="USB-C Port Soldered" width="300" />

#### 5. Button up

Do a test fit, this includes making sure wire length is not too short or long. Make sure the port fits nicely in the housing and is properly supported by the battery tray. Make sure your wires are out of the way of screw holes and won't bulge too much. Put the USB-C port in it's hole and re-connect your shoulder buttons. Close the console fully and start your screws. For the screws nearest the port, make sure the shell is clipped together nicely before fully tightening the screws.

## Troubleshooting Section

Most of this is self explanatory but this is where I explain why the method listed above is better than others I have seen online.  

So other guides have you taking out the mainboard fully and soldering to the back of the charging port. I did this my first time and while it did work and the wires were shorter technically. It led to so many issues, firstly is that the top screen cable of a 3ds is very fragile so I had to replace my top screen. Not only that but taking out the circlepad can break the clip on the mainboard, meaning you have to figure out how to fix that.  

What I discovered (when it comes to the circlepad) is that there are 3 test points (and ground) that you can hijack if you break the ribbon cable or connector. This is shown in the picture below.  

<img src="/images/IMG_0936.JPEG" alt="Circlepad Fix" width="300" />

The top pin is ground and any ground pad will work. The other three are (assuming) power, x and y input. I had to use a multimeter to find these and now my circlepad works consistently again (thankfully).  

#### My USB-C port doesn't work!?!

This is most likely caused by the wire not being soldered in properly. Use a multimeter and check for continuity from the breakout board to the mainboard.

#### My shoulder button doesn't work

This is caused by the breakout board being too close to the button. The solution I found is to take out the shoulder button and trim it so it no longer catches on the breakout board.

## FAQ

#### How does this actually work?

So we hijack the VCC and GND lines of the original port which means we retain the original port's charging. This means that the C port is ONLY for power, not data or other functions. This is a convenience mod.

#### Can you do this on other consoles?

Potentially, I am not for sure yet as I have just done this on the NEW 3DS XL. The main problem will be finding space in the case for the board to sit.

#### Does this do voltage regulation?

Surprisingly, yes. The mainboard handles voltage regulation, meaning any charger should work in theory. I have tried with a 19V laptop charger which didn't fry it. 5V desktop or from a power brick is preferred though, as I don't trust the voltage regulation **that** much.

#### I have a question that isn't listed

DM me on either Twitter (@IcyLetters) or on here and I will try to get back to you ASAP.
