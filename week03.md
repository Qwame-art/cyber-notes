Week 3: Windows and files: the OS, folders, users, file signatures, hashes and searching
## Day 1: Week 2 fixes, then what an operating system does
The 5 Jobs of an Operating System
1. Process Management: The operating system manages running programs and ensures they get the resources they need.
2. Memory Management: It controls how the computer's RAM is allocated and used by different programs.
3. File Management: It helps users create, save, organize, find and delete files and folders.
4. Device Management: It controls hardware devices such as printers, keyboards, monitors and storage devices.
5. User Interface: It provides a way for users to communicate and interact with the computer.


gmail.com  MX preference = 5, mail exchanger = gmail-smtp-in.1.google.com


| Hops in total | Hop 1 address | Hop 1 = my gateway? | Lines with * * * | Times on the last line |
30                13                yes                   line 2 and 6        90ms 44ms 50ms  

Windows 11
version  number 26H2 
OS Build number (OS Build 26300.9974)

Processor : intel(R)core(TM)i5-8350u CPU @ 1.70GH
Installed RAM : 16.0GB
Sytem type : 64-bit operating system,x64-based processor
Edition : Windows 11 pro



## Day 2: Windows: editions, the folder tree, NTFS, users and UAC
        Important Windows Directtories

  1. C:\Windows\System32 - Contains important Windows system files and tools needed for the operating System to function.

  2. C:\Users\<you>-Contains a user's personal files, such as Documents, Downloads,Dessktop and Pictures.

  3. AppData - Store application settings, preferences and other application-specific data.


   folders and your account
**Windows Account:** My Windows username is my personal account name.

**Account Type:** Administrator.

**Why is a Standard Account Safer?**

A Standard account is safer for everyday use because it has limited permissions. This reduce the risk of unauthorized system changes, accidental damage and malware gaining administrative privileges.


#Activity 3: Inspect Hidden Folders

I opened the AppData Roaming folder using %appdata%.

Three folders found:
1.Code
2.Kingsoft
3.JetBrains
These folders contain application-specific-settings,configurations and user data.

4822
Why is deleting unknown files from system32 a bad idea?
Because System32 contains essential Windows system files, and deleting important files can cause Windows or applications to malfuncttion.

User Accounts.
.My Windows account is an Administrator account.
.A standard account is safer for everyday use because it has limited permissions, reducing unauthorized system changes.

User Account Control
UAC is a Windows security feature that asks for permission or administrator credentials before allowing certain changes that require elevated privileges.



## Day 3: Files: bytes, extensions, signatures, hex and hashes
Same Bytes, New Name

a. First row of Format-Hex note.txt: 41 6B 77 61 61 62 61 0D 0A 

b. first row of Format-Hex note.jpg: 41 6B 77 61 61 62 61 0D 0A

c. Did renaming change any byte?
No. Renaming did not change any byte.
This shows that changing a file extension changes its name , not its actual contents or format.


One Letter,New Hash
a. Original hash(first 8 symbols):0EEA137F

b. New hash after adding an exclamation mark:E37DE810

c. Why is checking hashes useful for downloads?
checking hashes helps verify that downloaded files have not been altered and match the original file provided by a trusted publisher.


Hexadecimal by Hand 

Hexadecimal        Decimal   Character
4D                 77        M
5A                 90        Z
25                 37        %

What is a file starting with 4D 5A
it is commonly a Windows executable file with the MZ file signature.


## Day 4: Windows' built-in tools: processes, services, startup, registry, logs
Identifying a Fake Svchost.exe are:
Two ways to identify a fake svchost.exe are:
1. Check the spelling: The legitimate Windows process is named exactly svchost.exe. Misspellings or unusual characters may indicate a suspicious file.

2. Check the location: The legitimate process normally runs from C:\windows\System32. A copy running from an unexpected folder should be investigated.

Conclusion: Checking the exact filename and its folder location helps identify suspicious processes.


Windows' own tools, on your laptop

System Information
-Os Name: Microsoft Windows 11 pro
-Version: 10.0.26300 Build 26300
-BIOS model: UEFI
-Secure Boot State: On

Secure Boot is enable, which matches the recommended safe setting because it helps prevent unauthorized software from loading during startup.


STARTUP APPS
App Name            Publisher              Status
Microsoft Teams     Microsoft             Enabled
Mobile devices      Microsoft Windows     Enabled
Phone Link          Microsoft Corporation  Disbled


Event Viewer
-Date and Time: 11/20/2026, 7:11:05 pm
-Source : WindowsUpdateClient
-Event ID: 20
-Description: Event Id 20 indicates that Windows failed to install an update successfully.


-Error Code: No error code was displayed in the general tab.
-Meaning: Windows Update encountered an installation problem, but the specific error code was not available.


Running Services
-Number of running service: 135

**Difference between a process and a service:**
A process is a running program, while a service is a backgroung program that perform specific system or application tasks.



