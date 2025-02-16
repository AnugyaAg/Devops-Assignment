# DevOps Assignment: Version Control Systems
## Subversion (SVN)
Subversion (SVN) is an open-source version control system that allows users to track changes, revert to previous versions, and merge new features efficiently.
### Types of Version Control Systems:
  - **Centralized Version Control System (CVCS):** A single central server stores all versions.

  - **Distributed Version Control System (DVCS):** Each user has a full copy of the repository.
### Why Use Version Control?
 - Track all changes and maintain history.
 - Rollback to previous versions when necessary.
 - Merge new features seamlessly.
 ### Installing & Setting Up SVN on Windows:
1. Download and install SVN (TortoiseSVN).
2. Restart your system after installation.
3. Verify the installation using:
   
   ```sh
   svn --version
   ```
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%201.png)

### SVN Commands
#### Step 1: Initialize the Repository
```sh
svnadmin create ~/svn_repo/my_project
```
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%202.png)

#### Step 2: Checkout the Repository
```sh
svn checkout file:///path/to/svn_repo/my_project
```
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%203.png)

#### Step 3: Add Files to the Directory
```sh
cd my_project
svn add file.txt
svn commit -m "Added file.txt"
```
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%204.png)
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%205.png)

#### Step 4: Update Your Working Copy and View Logs
```sh
svn update
svn log
```
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%206.png)

#### Step 5: Reverting Changes
```sh
svn revert file.txt
```
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%207.png)

#### Step 6: Creating a Branch and Merging Changes
```sh
svn copy file:///C:/svn_repos/my_repo/trunk file:///C:/svn_repos/my_repo/branches/feature-branch -m "Creating feature branch"
svn merge file:///C:/svn_repos/my_repo/branches/feature-branch
```

---
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%208.png)
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%209.png)

## Mercurial (Hg)

Mercurial is a distributed version control system (DVCS) designed for efficient handling of projects of all sizes. It is similar to Git but focuses on simplicity and ease of use. Written in Python, it is known for its intuitive commands, robust performance, and cross-platform compatibility.

### Features of Mercurial:
- **Distributed Version Control:** Each developer has a full copy of the repository, enabling offline work and independent branching.
- **Lightweight and Fast:** Efficiently handles large projects and binary files.
- **Cross-Platform:** Works on Windows, macOS, and Linux.
- **Extensible:** Supports plugins for additional functionality.
- **Simple and Intuitive Commands:** Consistent syntax and easy to learn.

### Installing & Setting Up Mercurial on Windows:
1. Download and install Mercurial (TortoiseHg).
2. Restart your system after installation.
3. Verify the installation using:

   ```sh
   hg --version
   ```
   ![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%2010.png)

   ### Mercurial Commands
#### Step 1: Creating and Initializing the Repository
```sh
hg init my-hg-repo
```
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%2011.png)

#### Step 2: Adding and Committing Files
```sh
hg add file.txt
hg commit -m "Added newfile.txt"
```
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%2012.png)

#### Step 3: Cloning, Updating, and Reverting
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%2013.png)

```sh
hg clone https://example.com/repo
hg pull
hg update
hg log
```
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%2014.png)
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%2015.png)

#### Step 4: Branching and Merging
```sh
hg branch new-feature
hg merge
```
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%2016.png)
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%2017.png )
![Example Image](https://github.com/AnugyaAg/Devops-Assignment/blob/main/Screenshot%2018.png)

## Conclusion
Version control systems like **Subversion (SVN)** and **Mercurial (Hg)** help developers efficiently manage code, track changes, and collaborate seamlessly. Understanding these tools ensures better project management and smoother workflows in software development.

Happy coding! 🚀

