sheep_eid
=========

Sheep EID Reader Hardware

Goal is to develp an inexpensive set of reader hardware for reading official sheep RFID or Electronic ID tags. 

We're looking at 3 hardware pieces, reader, handheld tablet or phone and desktop. This project documents the reader device development.

Pix of the current state of the device are here:

http://www.flickr.com/photos/26001709@N03/sets/72157631585185604/

We used plumbing parts to make the holder for the reader and have a terminal program running on the Android tablet that is just displaying the tag numbers as read. 

No smarts, no database nothing really but verifying the hardware is working. 

More info on the existing state of the system:

RFID Reader:

http://www.priority1design.com.au/shopfront/index.php?main_page=product_info&cPath=1&products_id=24

Antenna is included.

Bluetooth Serial module:

For prototyping:

http://www.ebay.com/itm/Arduino-Wireless-Serial-4-Pin-Bluetooth-RF-Transceiver-Module-RS232-w-Backplane-/271040855319?pt=US_USB_Bluetooth_Adapters_Dongles&hash=item3f1b4b3d17

For production: (needs FCC cert, the above ones from China are real
cheap, but no certs.)

https://www.sparkfun.com/products/10253

Battery holder:

https://www.sparkfun.com/products/551

This one holds 4 cells, I used one that held 6. 4 is ok for this purpose
as the RFID reader can take 6-16V as an input. Should run for a couple
of hours on these batts, maybe use rechargeable NiMH or LiIon's for
production.

Misc.:

switch, led's 2 1k resistors, wire, various PVC fittings ($10US worth,
although the switch was surplus and probably cost a lot originally)

You could use GetBlue right now to do a good job of logging tags:

http://www.tec-it.com/en/software/android/getblue/manual/Default.aspx

the free version works ok (with nags), paid it's $25US and can save all
the tag data to a file or stuff it into a database or whatnot.

Our app will be completely open (GPLv2)

The Bluetooth API for Android already works well and there are open
source apps that use it successfully to read GPS's and the like.

This is where we are starting:

http://pymasde.es/blueterm/
