This is a BT 3.0 SH plugin to run an Estimote iBeacon on iOS 6 devices.

I needed this to test iBeacons on older phones.

To use this plugin


1) update the name of the class to your custom class 

eg: change AT_BlankScreenA to your class name

2) Update your appDelegate

eg: from BT_appDelegate to yourappname_appDelegate

3) change the custom class of the .xib file

eg: change AT_BlankScreenA to your class name


Use the AT_BlankScreenB class to create a plugin to detect Estimote iBeacons on iOS 6 devices.





beacons-demo
============

Simple demo apps to simulate Apple iOS7 iBeacon feature on iOS6 devices.

In order to make the Broadcaster and Receiver apps communicate smoothly you should generate your own BLE service and characteristic UUIDs:

+ open Terminal app, run «uuidgen» to generate a UUID
+ assign the UUID value to SERVICE_UUID in BluetoothServices.h in *both* projects
+ run «uuidgen» once again to get a new UUID
+ assign the new UUID value to CHARACTERISTIC_UUID in BluetoothServices.h in *both* projects
