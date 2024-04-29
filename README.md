# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript      
NAME:Revathi K  
REG.NO: 212223040169

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


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/Revathikuppan/Windows-basic-commands-batchscript/assets/144870694/d8b1199a-8eba-4ad1-9341-c38876f4cdbe)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/Revathikuppan/Windows-basic-commands-batchscript/assets/144870694/b5b13cbd-f505-4243-95f0-99dde02cd349)

![image](https://github.com/Revathikuppan/Windows-basic-commands-batchscript/assets/144870694/ff6bcb61-b581-40ef-8c59-667354050223)



List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/Revathikuppan/Windows-basic-commands-batchscript/assets/144870694/9eed9b36-fc0d-4483-8b24-f0a50b21d713)



Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/Revathikuppan/Windows-basic-commands-batchscript/assets/144870694/65b5e5b8-d646-4a32-92cf-c9d8da09390d)


![image](https://github.com/Revathikuppan/Windows-basic-commands-batchscript/assets/144870694/ffa08d8e-e7ec-4113-b4f7-8afed6d31be3)




Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/Revathikuppan/Windows-basic-commands-batchscript/assets/144870694/bdded770-11f0-48ef-a098-325bbac0092b)





## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```



## OUTPUT

![image](https://github.com/Revathikuppan/Windows-basic-commands-batchscript/assets/144870694/63a06d8e-c1d7-4ff0-ba2e-cb9982825c4b)




# RESULT:
The commands/batch files are executed successfully.
