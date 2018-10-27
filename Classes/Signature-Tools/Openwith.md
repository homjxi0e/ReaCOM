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
         S-1-15-3-1024-1065365936-1281604716-3511738428-1654721687-432734479-3232135806-4053264122-3456934681 Allow  ReadKey
Audit  :
Sddl   : O:SYG:SYD:AI(A;CIID;KR;;;BU)(A;CIID;KA;;;BA)(A;CIID;KA;;;SY)(A;CIIOID;KA;;;CO)(A;CIID;KR;;;AC)(A;CIID;KR;;;S-1-15-3-1024-1065365936-1281604
         716-3511738428-1654721687-432734479-3232135806-4053264122-3456934681)



PS C:\>
```
