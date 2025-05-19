# Windows-basic-commands-batchscript.

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
Create a directory named "My-folder" on the desktop.


## COMMAND AND OUTPUT
```
mkdir my-folder
```
![img](./img/Screenshot%202025-05-15%20182359.png)

## COMMAND AND OUTPUT
```
rmdir my-folder
```
![img](./img/Screenshot%202025-05-15%20182452.png)

## COMMAND AND OUTPUT
```
COPY CON Rose.txt
```
A clock in a office can never get stolen
Too many employees watch it all the time
^Z
1 file(s) copied
```
dir Rose.txt
```
![img](./img/Screenshot%202025-05-15%20182616.png)

## COMMAND AND OUTPUT
```
echo “hello world” > hello.txt
type hello.txt
```
![img](./img/Screenshot%202025-05-15%20182725.png)


## COMMAND AND OUTPUT
```
copy hello.txt hello1.txt
```
![img](./img/Screenshot%202025-05-15%20182831.png)


## COMMAND AND OUTPUT
```
del hello1.txt
dir hello1.txt
```
![img](./img/Screenshot%202025-05-15%20182917.png)

## COMMAND AND OUTPUT
```
assoc | more
```
![img](./img/Screenshot%202025-05-15%20182956.png)

## COMMAND AND OUTPUT
```
fc hello.txt Rose.txt
```
![img](./img/Screenshot%202025-05-15%20183038.png)

## COMMAND AND OUTPUT

Open Notepad with filename 1.bat and type the following batch scrip
```
    @echo off
    set name=John
    echo Hello, %name%!
    pause
```
![img](./img/Screenshot%202025-05-15%20183258.png)

## COMMAND AND OUTPUT

Open Notepad with filename 2.bat and type the following and execute 2.bat
```
    @echo off
    :main
    set /p number=Enter a number: 
    rem Calculate remainder when divided by 2
    set /a remainder=%number% %% 2
    if %remainder%==1 (
        echo %number% is an odd number.
    ) else (
        echo %number% is not an odd number.
    )
    :choice
    set /p continue=Do you want to check another number? (Y/N): 
    if /i "%continue%"=="Y" goto main
    if /i "%continue%"=="N" goto end
    echo Invalid choice, please enter Y or N.
    goto choice
    :end
    echo Thank you for using the odd number checker!
    pause
```
![img](./img/Screenshot%202025-05-15%20183452.png)


# RESULT:
The commands/batch files are executed successfully.

