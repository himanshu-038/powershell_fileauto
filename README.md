# powershell_fileauto
Folder monitoring and file extract automation using powershell scripts and windows batch file
The program does the following tasks:
1)	Monitors a folder (in this case 'C:\Users\Icon\Desktop\test\monitored') for any changes including deletion and creation of files for 2 mins (can be modified).
2)	When there is a change in the folder, it calls the function Invoke-SomeAction().
3)	The invoke-SomeAction() function displays the information about the change on the console and runs a batch file i.e. unzip.BAT.
4)	The batch file unzips the zip file into the specified folder i.e. C:\Users\Icon\Desktop\test\unzipped.
5)	At the end of 2 mins, it executes a .exe file i.e. C:\Program Files (x86)\USDA\RUSLE2\ARS\Rusle2.exe

The program used for unzipping is 7zip. It uses IO.FileSystemWatcher class object and methods to monitor the folder.

