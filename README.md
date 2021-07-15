# maxautoscriptsync
Maximo Automation Script Utility

1	Introduction 
As part of the Maximo development community, some of the drawbacks with automation scripting have been around organizing the scripts by objects. Finding scripts from the UI accurately and quickly can be attributed to tribal knowledge at best. To pile on the inconvenience, creating a new script or updating a script is a process and would require multiple windows to change and test.
To improve productivity, the Automation Script Sync tool was built to overcome these challenges. The Automation Script Sync tool will help the Maximo Developers to do the following: 
a.	Download the existing automation scripts from a Maximo Server and organize it into a tree folder structure based on type, objects and launch points. 
b.	Create or update the scripts back to the server.
2	Prerequisites 
a.	Create an object structure for the AUTOSCRIPT object with child object SCRIPTLAUNCHPOINT. 
b.	The OBJECTEVENT attribute should not be restricted under the SCRIPTLAUNCHPOINT object.
3	Instructions
3.1	Configuration Settings
a.	Update all the values in autoscriptutil.ini files with relevant values.
b.	Ensure the user provided has access to the object structure via OSLC.
3.2	Download Scripts
a.	Click the autoscriptsync.exe file.
b.	Follow the user prompt and select 1 to Download.
c.	Use the options to download all the scripts or a specific script.
3.3	Sync Scripts
a.	Update a script or create a new script in the tree structure as downloaded in the above steps.
b.	Click the autoscriptsync.exe file.
c.	Follow the user prompt and select 2 to Sync.
d.	Enter the script to be synched.
e.	If the script exists on the server, then script is updated. A new script is created otherwise. Follow the instructions prompted to create the launch point.

4. Limitiations
a.  Currently supported in Windows only
b.  Integration Scripts cannot be created from the utility. Create the integration script in Maximo to edit the same in the tool


