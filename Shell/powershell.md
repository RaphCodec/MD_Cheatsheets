# PowerShell Cheatsheet

## Introduction
PowerShell is a powerful scripting language and command-line shell developed by Microsoft. It provides a wide range of features and functionalities for managing and automating tasks in Windows environments.

## Basic Commands
Here are some basic PowerShell commands to get you started:

- `Get-Process`: Lists all running processes.
- `Get-Service`: Retrieves information about services.
- `Get-ChildItem`: Lists files and directories in a specified location.
- `Set-Location`: Changes the current location in the file system.
- `New-Item`: Creates a new item, such as a file or directory.
- `Invoke-Item`: Opens a file or launches an application associated with the file.

```powershell
Get-Process
```
```powershell
Get-Service
```
```powershell
Get-ChildItem
```
```powershell
Set-Location
```
```powershell
New-Item
```
```powershell
Invoke-Item -Path "C:\path\to\file.txt"
```

## Variables
In PowerShell, you can assign values to variables using the `$` symbol. Here's an example:

```powershell
$myVariable = "Hello, World!"
```



## Control Flow
PowerShell supports various control flow statements, including `if`, `else`, `elseif`, `switch`, `foreach`, and `while`. Here's an example of an `if` statement:

```powershell
if ($condition) {
    # Code to execute if the condition is true
} else {
    # Code to execute if the condition is false
}
```

## Functions
You can define your own functions in PowerShell using the `function` keyword. Here's an example:

```powershell
function SayHello {
    param (
        [string]$name
    )

    Write-Host "Hello, $name!"
}

SayHello -name "John"
```

## Modules
PowerShell modules are self-contained packages that contain reusable code. You can import modules using the `Import-Module` command. Here's an example:

```powershell
Import-Module MyModule
```

## Conclusion
This cheatsheet provides a brief overview of PowerShell and its basic features. For more detailed information, refer to the official PowerShell documentation.
