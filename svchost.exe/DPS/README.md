### svchost.exe | DPS
> Short for Diagnostic Policy Service.
**NOTE: You do not need a kernel driver to read and or write memory from this process, like some other processes.

### Explanation
> Diagnostic Policy Service resides as a core service within svchost.exe 

> On Windows, you've probably ran a portable executable. These executables have headers that contain information like the compilation timestamp, which is a 32-bit value, representing the time passed since Unix epoch. 

> More likely then not, an executable isn't going to be recompiled every single download-though it is possible and there are instances of this occuring. This process isn't always reliable in detecting cheats or malware. If you can that the timestamp of one executable isn't modified and matches the same executable from another source or download, only then is it a good indication that the timestamps match, and is likely that executable is what you put out to be. (It's also very unlikely that you have the exact same timestamp as some random executable on your computer, unless spoofed)

### Steps
> 1. Open up System Informer (or your application of choice)
![img](img/1.png)

> 2. Once open, filter or search for the process name. In this case, since System Informer is amazing, you won't have to hover over every single svchost.exe process running. You can just simply type DPS, which narrows it down a ton.
![img](img/2.png)

> 3. Open the properties of the process. Easiest way of doing this is double clicking the process, or right clicking, then finding the "Properties" button.
![img](img/3.png)

> 4. You'll be prompted a new window, the properties window. In this window, you should see the memory tab. Click it once to display the base address, types, size, and other properties of memory in MsMpEng.exe
![img](img/4.png)

> 5. Now, we want to click the "Strings" option which will prompt a new window. In the window, we should edit the filters for the string search. Ensure that the minimum length is 4, and ensure that the only checked boxes are 'Detect Unicode', 'Private', 'Image', and 'Mapped'
![img](img/5.png)

> 6. Now, press 'OK'. There should be a new window prompted, filtered with what we inputted last step. We're going to want to narrow our search even further, so we're going to click 'Filter', then 'Contains (case-insensitive).
![img](img/6.png)

> 7. Once again, a new window titled 'Filter' pops up, telling us to enter the filter pattern. Here, it gets somewhat local. Say, you ran a cheat (or any executable in that matter) that you know is a signed executable. For an example, I'll run 'Process Hacker 2' as an administrator, signed by 'Wen Jia Liu.' In the filter, I'll search for 'Wen Jia Liu' and press enter. If 'Wen Jia Liu' show ups in any form, this indicates that the executable I ran, 'Process Hacker 2', was ran in the instance of this Windows until reset of the computer, reset of the service MsMpEng.exe, or shutdown.
![img](img/7a.png) ![img](img/7b.png)

### Additional Notes
> Note that if I hadn't ran the executable from the time frame I start my computer and login, nothing would've shown as the process wouldn't have to scan the file and its signatures. One more note, the name of the publisher does not change unless the developer finds a way to spoof it for everytime their program is downloaded or compiled. This means that if person A, person B, and person C both have 'Process Hacker 2', the publisher's name is going to be the same. This applies the same way to cheat executables and or malware if signed.

![img](img/8.png)
