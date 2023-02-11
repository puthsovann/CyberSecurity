***Forensic*** -- Information security is a very crucial aspect of business management that has always remained at risk of attack. Once a system is compromised, it loses its confidentiality, integrity, and, at times, availability which damages normal business processes. Tragic as it may sound, all is not lost; sophisticated attacks take time to mature, giving a keen administrator a chance to detect an attack in its early stages and counter it soon enough. There are certain things you can look into when you suspect one of your machines is compromised. We have listed 14 things to check when a system gets compromised. Let’s list them one after the other.

There are two basic concepts used to examine a system that has been compromised:

***14 tips possible ways to counter attacks, You need to check for****

## 01. Unusual accounts created
Administrator accounts in the AD groups are the first thing to check when a system gets compromised. Because administrator accounts are used to perform activities that require special permissions, such as installing and configuring software or managing access controls and firewalls, there being presence of unknown accounts in the administrator’s group would imply an unknown user with complete control of a computer system. This is harmful to information security and should be controlled by performing regular audits to verify user authenticity. run a malicious attachment which may provide an attacker a foothold into the network.

*To remove administrator rights from an unknown account if encountered on a Windows 10 Pro or Enterprise computer.*
1. Press together win+R keys to open Run. Type the command lusrmgr.msc on Run and click OK
2. Tap on ‘Groups‘ on the displayed pane and select the administrator’s groups
3. Right-click the admin group and select their properties
4. Select the individual user you wish to eliminate and tap on the ‘Remove’ button

## 02. Unusual Big Files on storage > 5GB
Another common sign of a compromised system is the presence of unusually large files(5GB) or more. Said files show up in your storage, totally unaware of all other users in your system. Whenever you notice such an extensive and curious database read in your system storage, it means that hackers have already infiltrated your system and are now gathering up your data to steal it. Check for large files is another thing to check when a system gets compromised.A remedy hereby would be to immediately delete the folders and install an anti-virus for constant checks.

## 03. Any unusual files added recently in system folders
To launch malware into your system, attackers usually plant a file in your system and induce you to open it. Documents containing such malicious code are heavy and subtly hidden as Microsoft documents to appear legitimate.
Search for any unknown or suspicious file types. An efficient way to handle this would be to run a virus scan and ensure all malware is removed.

## 04. File using the "Hidden" Attribute Property
Any file with a Hidden attribute turned on during property settings is a hidden file. These files are not displayed when their location folder is opened with Windows Explorer or searched on the local machine.
Windows traditionally used the hidden attribute to set apart various crucial program files and keep them safe for modification. This attribute has traversed modern cyberspace and is now being used by hackers to evade detection. So checking for hidden files is an obvious thing to check when a system gets compromised.

## 05. Unusual Programs Launched at Boot time in Window Registry
Yet another way of discovering a swystem under compromise is discovery strange programe running during machine boot time. So, never forget this thing to check when a system gets compromise. To check what programs are getting launched at boot time: 
1. Open the ***task manager***
2. Select the ***startup tab*** on the window that pops up.

A list of programs should be indicated, and in case you find one looking suspicious or lacking a publisher unlisted, right-click it. You will be prompted with the options to open the file location, study its properties or disable it.Advisably disable the program, but if that option is greyed out, you can alternatively right-click on one of the tabs displayed and enable the command line.Now you can see the full path to the programs running and take appropriate action. However, having a reliable anti-virus installed is more full-proof, meaning protection will require fewer manual interventions.

## 06. All Running Process for unusual/unknown entries, especially with users "System" and "Administrator"
Whatever may be the program is, legit or malicious. Everything just runs as a process. But, the fact is, It is very easy to lose track of processes running on your windows server system. At any particular time, hundreds of processes, schedules, handles, and privileges operate simultaneously, and a spooky program could be launched and go unnoticed for a while. Process monitoring plays a crucial role in the malware detection process. You shouldn’t leave this thing to check when a system gets compromised.

To get a full display of all running processes, open the ***taskbar***, and it automatically lands on the ***processes tab***. Alternatively, typing ***‘tasklist‘*** on the command line should display them and right-click to end task.

The ‘tasklist’ command is helpful but does not give you a text file of the running processes. Instead, type the command ***‘tasklist > c:\process_list.txt’ to get a saved copy.***

## 07. Check User’s Autostart Folders
Window computers have the ability to configure apps and have them run automatically anytime your system boots up. The startup folder for all users sharing a computer can be accessed through the path ***C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp***, and the path for individual users is accessed through ***C:\Users\username\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup*** (replace username with actual user account name).
Once on the folders, you should add a shortcut of your desired app to the startup folder. It is worth noting that there are two startup folders on any shared computer, one for all users and another for individual users. That said, each user can customize it to their preferences.

Whenever you find a suspicious folder placed under autostart in your computer system, disable them by the following steps;
1. Open the task manager
2. Open the startup tab on the window that opens
3. Disable any unauthorized programs running in your startup

Alternatively, the best way to open Startup folders in windows is to run the address shell:startup the Run-Dialog box(Windows key+ R) and delete the folders.

[More](https://thesecmaster.com/14-things-to-check-when-a-system-gets-compromised/)


