# localization-wifi
A simple application for indoor localization using wifi fingerprinting

** Files in /src/data **

There are two folders in /src/data. One contains our own built reference data along with measurements. The other folder contains assignment's reference data with our measurements.

The reference data should be present in internal storage location /Android/com.group20.assignment2.mobilesensing/files in order to be used by the application.


** Files in /src/MobileSensing **

The .java files for each Activity is present in 

/src/MobileSensing/app/src/main/java/com/group20/assignment2/mobilesensing/

Following is the description of all the activities

1. ListSensorsActivity.java - This activity will list all the sensors on the mobile phone along with OS and manufacturer information.
2. LocalizationActivity.java - Gives an interface to compute location of a measurement. Also allows creating, updating, deleting measurement data. We can also create reference data thru this activity.
3. MainActivity.java - List all the links to respective activities
4. ViewReferencePointsActivity.java - This activity will list all the reference locations and show their WiFi fingerprints
5. ScanWifiActivity.java - Scans wifi APs around and lists them.

Classes

1. LocationPoint.java - This class signifies a location point. An object of this class can be a measurement location or a reference location. It has a method to calculate euclidean distance from another location point.
2. WifiAP.java - Stores details of a wifi access point (BSSID, SSID, level, etc.)



** HOW TO USE THE APP **
After building the apk and installing it, the main activity will run. Select appropriate link to run respective activity.
The localization activity will show all the measurements and their computed locations.

To obtain a new measurement of current location's wifi fingerprint, click CREATE button. 

To update the measurement click UPDATE

Click SAVE AS REFERENCE to create a new reference from the current measurement.

Click VIEW REFERENCE to view all the created references.