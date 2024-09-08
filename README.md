# AppleWatchAmmeter
Turn your Apple Watch into an ammeter to measure DC currents.

Apple Watches newer than Series 5 which contain a compass also contain a magnetometer. The magnetometer is also sensitive to magnetic fields from nearby currents.

This demonstration uses a coil of wire around the watch to alter the magnetic field sensed.

An app could easily be written to perform some calibration and zero offset as well as display curent in Amperes. however nearly any app that can display raw magnetometer data can be used. I use 'Sensor-App' which is free.

In this demonstration, a 6-turn coil can easily show curent changes of about 10 mA.

The Earth's background magnetic field is around 60 uT (not only in a North-South direction). With a 6-turn winding, each 1 A generates an additional ~ 100 uT in the Z direction; there is some noise in the readings, but with care, 10 mA (1 uT) changes can be discerned.

<img width="483" alt="Watch Ammeter" src="https://github.com/user-attachments/assets/7a0e5de4-8679-49e0-82f7-6bd6a99a204e">

<img width="630" alt="Watch Ammeter winding frame" src="https://github.com/user-attachments/assets/0a09424d-a807-4526-8fa3-dc72502a79d3">

