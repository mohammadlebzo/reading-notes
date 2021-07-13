# A summary about ***Git***: What is it and How does it work ?

### Introduction:

Before I can start explianing what is **Git**, and how it works, i need to first explian a cuple of 
terms that will help later in properly explianing what is **Git**.

- #### **Version Control System (VCS)**:
Version Control Systems are basically a ***history of all changes on the file*** and its represented as ***versions*** of that file.


- #### **Local Version Control System (LVCS)**:
Local Version Control Systems are basically ***the history of file versions located on the user's hard drive***.


- #### **Centralized Version Control System (CVCS)**:
Centralized Version Control Systems are basically ***a way for collaborators to work together on a single
file stored on a server***.


- #### **Distributed Version Control System (DVCS)**:
Distributed Version Control Systems are basically ***hybrid systems that are used by collaborators, and they use both (LVCS) and (CVCS)***, meaning that each of users have a clone of the file locally on their machine, and they can push modifications on a centralized machine (server) for other users to pull and use.


### Now, what is ***Git***?

**Git is a (DVCS) that stores data in a file system made up of snapshots**. <br>Each time you save a changed version of your project ***called commit*** Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

### Some ***Git*** commands:

**To add changes for all files:**
```
git add .
```
**As for one file:**
```
git add fileName
```
**To commit changes on files:**
```
git commit -m"Comment about the changes"
```
**To push the changes: (i will use the main branch)**
```
git push origin main
```
The user will be asked to add the github **username** and **password** only if the used format is ***https***.
**To pull the latest version contant: (i will use the main branch)**
```
git pull origin main
```