# AppleWatchAmmeter
Turn your Apple Watch or any watch with an accessible magnetometer into an ammeter to measure DC currents.

Apple Watches newer than Series 5 which have a compass also contain a magnetometer. The magnetometer is also sensitive to magnetic fields from nearby currents.

This demonstration uses a coil of wire around the watch to alter the magnetic field sensed. A circular coil of wire with N turns and a diameter D will generate a magnetic field of B = u0.I/D (u0 is defined to be 4.π.10^-7); so for a watch with a diameter of about 48 mm (approximately Apple Watch 5), 5 turns with 1 A will generate a field of 5 * 4.π.10^-7 * 1/0.048 = 131 uT (or 1.3 gauss). Because the magnetometer is not centered in the coil (it's usually in the very bottom right corner of the watch), the actual sensitivity is a bit lower; 100 uT/A is a reasonable approximation that can be improved by calibrating.

An app could easily be written to perform some calibration and zero offset as well as display current in Amperes. however nearly any app that can display raw magnetometer data can be used. I use 'Sensor-App' which is free. Note that you can only detect DC currents; the magnetometer is too slow to react to AC (e.g. household power) currents.

In this demonstration, a 5-turn coil can show curent changes of about 10 mA (about 1 uT in the Z direction).

The Earth's background magnetic field is around 60 uT (not only in a North-South direction). With a 5-turn winding, each 1 A generates an additional ~ 100 uT in the Z direction; there is some noise in the readings, but with care, 10 mA (1 uT) changes can be discerned. The Z-axis readings change linearly with current (either positive or negative), but also with nearby magnetic objects, so try not to move those as you make readings. Here's a chart of Z-Axis reading vs. current in a 5-turn coil. It's extremely linear:

![Apple Watch 5 44 mm Ammeter Chart](https://github.com/user-attachments/assets/4cb8e060-b12a-40df-8ab7-e9eea1688b61)


<img width="483" alt="Watch Ammeter" src="https://github.com/user-attachments/assets/7a0e5de4-8679-49e0-82f7-6bd6a99a204e">

<img width="998" alt="Coil holder with wires" src="https://github.com/user-attachments/assets/f63312f5-ba97-4c33-8e38-28b9935bb610">
