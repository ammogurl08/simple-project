# AtomProject package

A package that saves your project to a file which contains relative paths to all opened directories inside the project, which makes it easier to migrate your project file along with your directories.

## Example
E.g., you have a project that contains 3 directories:

- C:\Workspace\ProjectA\Folder1\scripts
- C:\Workspace\ProjectA\Folder3\scripts
- D:\Workspace\ProjectB

And your project file saves to **C:\Workspace\ProjectA\my.simple-project**

The content of **my.simple-project** file would be:
```
["Folder1\\scripts","Folder3\\scripts","D:\\Workspace\\ProjectB"]
```
If you migrate **ProjectA** folder to **D:\Workspace**, the project will still work.