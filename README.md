# Railuino-0.9.0
 Version 0.9.0 de la bibliothèque Railuino de Joerg Pleumann dont le dépôt git se trouve à cet emplacement : https://code.google.com/archive/p/railuino/

Cette bibliothèque est sous licence GNU LESSER GENERAL PUBLIC LICENSE - Version 2.1, February 1999

Copyright (C) 2012 Joerg Pleumann
![image](https://github.com/user-attachments/assets/50088613-c513-4d5b-9a5d-ecc6e12778e1)


Railuino - Hacking your Märklin

This library allows you to control your digital Märklin railway
using Arduino. It can be used in two flavors:

(1) As a Mobile Station 2. You can use a Sparkfun CAN shield and a
    cable to connect your Arduino to the Digital Connector Box of
    a Mobile Station 2 and probably (untested) also to a Central
    Station 2. This allows you to control locomotives, functions
    and turnouts using MM2, DCC and other protocols. You can even
    read and write decoder CVs, as long as the decoder's protocol
    supports it (DCC does both, MM2 only write, others vary).

(2) As an infrared controller. You can use a simple infrared LED
    and a resistor to have your Arduino talk to the very basic IR
    receiver box that comes with various starter packages. This
    allows you to control four MM2 locomotives on fixed addresses
    (the classic Delta addresses). You can also control sixteen
    turnouts (this is an undocumented feature of the IR box, and
    the original Marklin IR controller doesn't support it).

In addition to controlling things on and connected to the track
the library allows you to receive reports about track usage using
the standard S88 bus.

Installation is easy: Just get the latest release from the
downloads page and place the contents of the "src" directory in a
"Railuino" directory under your Arduino "libraries" directory.
Then restart Arduino. You should now see a bunch of new examples
that teach you how to use Railuino. The "Misc/Tests" example is
a good way of validating your setup.

For documentation on the functions I currently recommend to read
the comments in the "Railuino.h" header file. There are also
several sets of slides on the downloads page that describe the
overall approach and the hardware. Finally, there is a video from
LinuxTag and another one from DroidCon NL on YouTube.

The library itself is made available under the GNU Lesser General
Public License (LGPL). See the LICENSE file for details. All
examples except the test suite are licensed under the Creative
Commons Zero license, which effectively makes them public domain.
The test suite is also licensed under the LGPL.

Railuino uses parts of two other libraries, both of which are
very much recommended:

1) The CAN controller code is based on Fabian Greif's CANlib,
   which is (c) 2007-2012 Fabian Greif and licensed under a
   BSD-style license.

2) The IR sender code is taken from Ken Shirriff's IR library,
   which is (c) 2009-2012 Ken Shirriff and licensed under the
   GNU Lesser General Public Library. 

Have fun!
