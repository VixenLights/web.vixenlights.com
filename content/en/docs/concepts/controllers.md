---
title: Controllers
author: Jeff
date: 2013-04-28T16:22:45+00:00
weight: 40
---
Controllers are the actual objects that send data out of the computer, in a specific format and transport method to real hardware in your yard.  After you've defined your elements on a high level, you'll need to set up at least one controller to output data to the real world.  You'll need one controller for each output of your computer.  There are different kinds of controller modules that correspond with real world hardware.  For example, the "Open DMX Output" controller will output one universe of DMX data using the protocol designed for the Enttec Open DMX based hardware dongle.

When you configure a controller, you need to first specify the type.  There are several supported output types that correspond with various real world hardware.  After defining the controller, you need to tell it how many channels it will have.  This needs to be the sum of all of the individual output channels of all actual devices connected to that port.  Most controllers also have some other information specific to that device that also needs to be defined.  For a Renard, it would be the Com Port, and Baud Rate; for sACN, it's the universes and addressing.  Some controller types have no configurable parameters, the Open DMX Output is one example.  It doesn't use a com port, and it has a fixed output size of 512 channels.

One common mistake is for users to define multiple controllers when you should only be using one.  Many hardware systems use a common data bus where data leaves the computer from one port and then travels down a data wire in and out of several controllers in a daisy chain configuration.  The Renard protocol is a good example of this.  If you have a chain of Renards (regardless of type) that all connect to a computer at a single port, you need to define only one controller for that whole chain.  DMX, sACN, ArtNet are also common examples of controllers that share a data bus.

On the other hand, if you have two Renard (or DMX, etc) wires connected to different ports on your computer, you need to define one controller for each data connection.  Each may have it's own number of channels, and own configuration parameters (baud rate, etc).

While it's beyond the scope of this article, it's important to note that some hardware supports multiple protocols.  For example, a Renard controller may be configured to run DMX firmware.  In that case it's a DMX device and needs to be configured using a DMX controller, not a Renard controller.

Similarly, there are protocol converters out there that convert from one protocol to another.  For example, the sACN to DMX/Renard bridge will take data in on the sACN protocol via ethernet, and convert and output that data in Renard or DMX formats.  In this case, you would need to define the controller as a sACN controller in Vixen.  Vixen doesn't care what happens to the data downstream once it leaves the computer.

Another common mistake is to configure all the channels your controller can technically handle. This occurs with e1.31 controllers that can support thousands of channels. If you are only using 500 channels of the 2000 your controller supports, you only need to configure the 500 channels in Vixen. You can always change the count later on as your display expands.