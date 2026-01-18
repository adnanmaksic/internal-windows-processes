### MsMpEng.exe
> Short for Microsoft Malware Protection Engine.
**NOTE: You need a kernel driver to read and or write memory from this process. The easiest way to do this is to enable the option in System Informer and run in administrator, or install Process Hacker 2 (as by default, it has it enabled).

### Explanation
> MsMpEng.exe resides as a core process within Windows Defender, the pre-installed antimalware on all Windows systems. This process actively scans files, memory, and network activity.

> More likely then not, unless disabled, or using another antimalware software: if a person is going to run an executable, whether a cheat for a game, or malware, MsMpEng.exe will scan the file.

> Some cheat developers will sign or publish their executable, some cheat or malware developers will obfuscate their code. Either or, MsMpEng.exe is likely to have traces of the signature or flag of the executable that was ran on the system.

### Steps
1. Open up System Informer (or your application of choice, but it's very important that the application you use has kernel-level privileges)

[image here]

2. Once open, filter or search for the process name. In this case, MsMpEng.exe

[image here]

3. Open the properties of the process. Easiest way of doing this is double clicking the process, or right clicking, then finding the "Properties" button.

[image]