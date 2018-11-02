### Abusing the COM Registry Structure (Part 2): Hijacking & Loading Techniques
TL;DR
There are several ways that attackers can leverage COM hijacking to influence evasive loading and hidden persistence.  A few examples include CLSID (sub)key abandonment referencing, key overriding, and key linking.
There are several programs and utilities that can invoke COM registry payloads including Rundll32.exe, Xwizard.exe, Verclsid.exe, Mmc.exe, and the Task Scheduler.  In the traditional sense, any binary that resolves non-existent and/or unreferenced COM classes can be potentially influenced (e.g. hijacked) for “unintended” loading.
Hijacking COM server binaries introduces a few interesting use cases (e.g. MMC).  Attackers can leverage the -Embedding switch to open GUI binaries in a hidden manner.
Defensive considerations include implementing robust Application Whitelisting policies, monitoring for unsuspecting command line usage (e.g. “-Embedding”) with a deviation from the proper parent process (e.g. svchost.exe), and the creation of interesting Registry keys (e.g. “TreatAs”, “ScriptletUrl”, etc.).


### Background

Not long ago, I wrote a blog post about [Abusing the COM Registry Structure: CLSID, LocalServer32, & InprocServer32](https://bohops.com/2018/06/28/abusing-com-registry-structure-clsid-localserver32-inprocserver32/) In that previous post, a few interesting techniques were discussed such as abandoned registry key discovery, COM hijacking, lateral movement, defensive evasion, application whitelisting bypass, and situational persistence.  In this follow-up post, we will take it a step further and focus on a few other hijack methods and evasive loading techniques.  Topics include 
 
- COM Hijacking Techniques

- CLSID Loading Techniques for Evasion & Persistence

- COM Server Misuse: Microsoft Management Console (MMC) Use Case

- Defensive Considerations


###                                               COM Hijacking Techniques
In order to load and execute a COM payload without registration, an attacker must influence the COM registry structure.  A way to do this is through a technique called COM Hijacking.  One of the best definitions for COM Hijacking comes from the Mitre ATT&CK Framework:
“The Microsoft Component Object Model (COM) is a system within Windows to enable interaction between software components through the operating system.  Adversaries can use this system to insert malicious code that can be executed in place of legitimate software through hijacking the COM references and relationships as a means for persistence. Hijacking a COM object requires a change in the Windows Registry to replace a reference to a legitimate system component which may cause that component to not work when executed. When that system component is executed through normal system operation the adversary’s code will be executed instead.  An adversary is likely to hijack objects that are used frequently enough to maintain a consistent level of persistence, but are unlikely to break noticeable functionality within the system as to avoid system instability that could lead to detection.”
