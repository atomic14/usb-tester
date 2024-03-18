This is a work in progress.

It's a nice simple USB cable tester - you can watch a background video on it [here](https://www.youtube.com/watch?v=qdNnukfTZgA).

[![Demo Video](https://img.youtube.com/vi/qdNnukfTZgA/0.jpg)](https://www.youtube.com/watch?v=qdNnukfTZgA)

The above video covers versions 1 and 2. The current version is 3.

![PCB](images/USB-tester-brd.svg)

![3D Render](images/USB-tester.png)

The BOM is pretty straight forward, 100 ohm resistors and whatever color LEDs you would like to use.

The USB sockets are these ones: https://www.lcsc.com/product-detail/USB%20Connectors_XUNPU-TYPEC-324-BCP24_C2835314.html

# The Story So Far

For the first version I used these USB sockets.

![USB Sockets With All Pins](images/108b5c1832be3960da550cbffb4c0ac2.webp)

These break out all the pins - but unfortunately half the pins are hidden under the socket so you can’t see if you have solder bridges or bad connections. That coupled with a couple of design errors made the first version of the board a bit of a failure.

![Version 1](images/d8b2b47facb7414ef64aa4557a05cce1.webp)

So for version 2 I opted to use these sockets:

![New USB Sockets](images/f357adea6322bd8ff907483c64156cb2.webp)

These are a lot easier to inspect. Half the pins a through hole and the other half are visible at the back of the socket.

It is still pretty hard to solder up and not get any bridges, but at least now we can see them easily.

![Ooops - A Solder Bridge](images/75436e83aa750f28d40d0b026173641d.webp)

Version 2 works pretty well, we can test various cables - for example here’s a good quality cable that should be able to for 40Gbps.

![Fantastic Cable](images/681ed0021d1976ebd5df42bbc0de532d.webp)

And here’s a cable that is ok for normal USB - but it’s not going to set the world on fire when it comes to speed.

![An OK Cable](images/83bb386b155339976bb5e3f81c93a617.webp)

I’ve got a new version under construction. With the previous two versions it’s been really hard to tell if the sockets are soldered on properly. So I’ve now broken out all the connections and can easily build a test jig to check for shorts.

![USB Break Out](images/31a0adfcc9acdafd6bcd9c37a8c6e983.webp)

