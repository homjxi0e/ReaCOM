## Author bohops
Synopsis: 
Microsoft Management Console is including the file to invoke CLSID to drag Scriptlet or payload anything you want to execute it
 
MMC.exe: 
MMC – CLSID Web Address Link
Though not nearly as exciting as the remote command execution/lateral movement technique, MMC can be used to invoke CLSID payloads for evasive loading and Run Key persistence.  Let’s setup our MMC console file to demonstrate this example

MMC – CLSID Web Address Link
First, we need to setup a CLSID link and save our configuration as a console file (.msc).  We can setup our basic payload by opening the MMC and the “Add/Remove Snap-In” window.  For simplicity, select “the Link to Web Address” snap-in to open the wizard, and input the hijacked/reference CLSID key for the “Path or URL” as shown in the following screenshot:

![mmc_1](https://user-images.githubusercontent.com/25440152/47956228-01a7ab00-dfaa-11e8-9f51-abc0f127308c.png)

Figure 11:  MMC Add Snap-In – Web Address Link (Click Image to Enlarge)
Next, create a name for the snap-in and select ‘Finish’ as shown in the following screenshot:

 
![mmc_2](https://user-images.githubusercontent.com/25440152/47956235-1126f400-dfaa-11e8-9526-25048e066bb1.png)

Figure 12:  MMC Add Snap-In – Add Friendly Name (Click Image to Enlarge)
This will create our “test” menu item under the “Console Root.”  By selecting the “test” menu item, the CLSID link will invoke accordingly.

 
![mmc_3](https://user-images.githubusercontent.com/25440152/47956248-31ef4980-dfaa-11e8-9783-eb64bc9552de.png)

![mmc_embedding](https://user-images.githubusercontent.com/25440152/47956249-3451a380-dfaa-11e8-9d5d-a883412072d8.png)
