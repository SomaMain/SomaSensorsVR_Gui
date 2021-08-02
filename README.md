# SomaSensorsVR_Gui
First release of the GUI for SomaSensorServer

Start steamVR first before connecting to the server.


#Connection Panel

Scan Port Button - Scans for devices connected through serial port. Select the one that your hub is connected to

BaudRate - Currently useless. Needs to run at 256000 to get 90+hz

# Trackers - Select the number of trackers you want to show up in steamVR.

  - 1 will allow you to use a single tracker as a hip tracker
  - 
  - 3 will give you a hip and feet trackers. 
  - 
  - 11 will show all joints. This is for checking all trackers and see if any are rotating incorrectly.
  - 
Connect button - Connects to the server

Disconnet Button - Closes the server.

#Profile Settings

Save Profile button - Save the current settings: Profile, Skeleton, skeleton position, smoothing factor, ground level, Z-rotation

Load Profile button - Load a different profile text file

Load Skelly button - Load a custom skeleton text file created by the SkellyGenerator : https://github.com/SomaMain/SkellyGenerator

Select Client button - Select the version of the Server you wish to use. This option will be saved inside the profile, so don't forget to save!

#Commands

Wake Button - Wake up the HUB once you are inside steamVR and the trackers have shown up

Calibrate button - When the trackers are aligned inside of you, hit the calibrate button and T-pose. After 5 seconds it will finish and you can move

Reset Skelly Button - Stand up straight before clicking this. It will set the skeleton to your current position. DOES NOT CHANGE ROTATION. Make sure to align your rotation

Set Smooth button - Smooth ranges 0.01 - 0.99 from no-smoothing to too-much-smoothing. The less smoothing, the faster your trackers will react, but with more jitter.

Set Ground - Sets the distance, into the ground, that your feet trackers will travel before stopping.

Z-Rotation Buttons - Rotate clock/counter-clockwise. Align your trackers in YAW so they rotate the same in VR as they do in real life.


#Battery

The large battery, in the top right, shows the average battery life amongst all trackers.

There are check-boxes for the: Neck, Chest, Left/Right Foot. Check these to tell the server which trackers you will be using. The default is the standard 5 trackers : Waist, L/R Thigh, L/R Calf

- Setting # Trackers to 1 will only show the Waist Tracker

Quit - Closes the GUI and Server (if it is open)
