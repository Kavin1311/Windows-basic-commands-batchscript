# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 

# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-10-22 044645](https://github.com/user-attachments/assets/f7a8a997-ed13-4556-8dcd-160c9186d8a2)

## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
cd %userprofile%\Desktop\MyLab
type nul > MyFile.txt
```
![Screenshot 2024-10-22 044709](https://github.com/user-attachments/assets/29199160-b1e1-44d3-aead-e0d9e224f150)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2024-10-22 045612](https://github.com/user-attachments/assets/69051a2a-3af3-49bc-aea8-289d63efc786)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2024-10-22 045625](https://github.com/user-attachments/assets/d401fdd1-ffee-4682-a3d3-10a48ae74ab3)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
move MyLab C:\Users\admin\Documents
```
![Screenshot 2024-10-22 045646](https://github.com/user-attachments/assets/d0abedcb-de35-407d-8f84-24fdda83175e)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\DocBackup\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT
![Screenshot 2024-10-22 044626](https://github.com/user-attachments/assets/c5086941-975e-4a4a-a3fe-a9420da58d5b)

# RESULT:
The commands/batch files are executed successfully.

