# Windows File Management

> Basic Windows file management with PowerShell

- [Webpage](https://denisecase.github.io/windows-file-management/)
- [Source](https://github.com/denisecase/windows-file-management/)

## Prerequisites

- [Windows Setup for Developers](https://github.com/denisecase/windows-setup)

## Organizing Files

Windows arranges files in a tree structure, with the C:\ drive typically at the root of the tree. 
If a computer has been partitioned into multiple drives, you may see other drive names as well.

We can use PowerShell to create, delete, and rename folders, sub-folders, and files. 
It's a powerful tool for organizing your files.

For example, you may create a folder for school, and from inside that folder, 
create a sub-folder for each of your courses.

## File Explorer

The Windows File Explorer is a graphical way of browsing files. 
Use this along with the PowerShell command line interface (CLI). 
Folders and files can be added, edited, and deleted in File Explorer as well.

## Basic PowerShell Commands

PowerShell offers aliases (shortened names) for common commands. 
The full name is provided for additional reference [1].

- mkdir - create new folder/directory [Create-Item]
- cd - change directory [Set-Location]
- cd .. - cd up to immediate parent (cd ..\.. to go up 2 levels)
- rm - remove [Remove-Item]
- rni - rename item [Rename-Item]
- ni - new item [New-Item]
- ls - list contents [Get-ChildItem]
- clear - clear the history of commands [Clear-Host]

## Open PowerShell in User Folder

Use File Explorer to open your user folder (e.g. C:\Users\acctname). 
Right-click on the folder itself (showing your account name) or in the white space off to the right. 

Select "Open PowerShell window here as administrator" from the context menu [2].

## Working with Folders

"Folders" and "directories" are the same and the terms can be used interchangeably. 
When using the commands, it can be helpful to think in terms of "directories".

1. In your default user folder, create a new folder/directory named "projects".
2. Try to create it again (the command should fail).
3. Change into your new directory.
4. Make several subdirectories.
5. Move into the first subdirectory.
6. Create an empty file (new item).
7. Create another child directory.
8. Rename it.
9. Delete it.
10. Back up to your projects directory.
11. Back up to your user directory.

```PowerShell
mkdir projects
mkdir projects
cd projects
mkdir proj1
mkdir proj2
mkdir proj3
cd proj1
ni README.md
mkdir startup
rni startup startingup
rm startingup
cd ..
cd ..
```

## Terms

- Drive
- File
- File Explorer - Windows program for browsing folders and files
- Folder / directory - a place to store files on your computerf
- PowerShell - powerful command line interface for Windows
- Tree data structure (every node has exactly one parent, except the root node with no parent)
- Windows 10 - popular operating system

## Next Steps

- See [Basic Tools for Web Development](https://github.com/denisecase/basic-tools-for-webdev)

## References

1. [PowerShell Docs](https://docs.microsoft.com/en-us/powershell/scripting/powershell-scripting?view=powershell-6)
2. [Windows Setup for Developers](https://denisecase.github.io/windows-setup/)
