# TITO_Trainning_Git

## Table of contents

### [Chapter 1. Introduction]()

### [Chapter 2. Creating Your Repositor]()

### [Chapter 3. Branching, Places and GUIs]()

### [Chapter 4. Merge, Pull Request and Handling Merge Conflicts]()

### [Chapter 5. Rebasing, Amend and Cherry-Picking]()

### [Chapter 6. Interactive Rebasing]()

### [Chapter 7. Workflow, Notes and Tags]()

### [Chapter 8. Aliases]()

### [Chapter 9. Using the Log]()

<br></br>

### Chapter 1. Introduction

- Git is a Distributed Version Control System - DVCS
- Developed by Linus Torvalds in 2005.
- Git is commonly used in source code management and software development document managementGit is commonly used in source code management and software development document management.
- Git allows team members to work together on the same project efficiently and conveniently.

<br></br>

### Chapter 2. Creating Your Repositor

<details>
<summary>1. Create a repository then write code </summary>

- Create a repository
- Pull the repository to your computer 

```
$git clone HTTPS/SSH
```

- Add the files 

```
$git add .
```

- Commit at the command line

```
$git commit -m "commit"
```

- Push code 

```
$git push origin branch
```

</details>


<details>
<summary>2. Create local project and push</summary>

- Create a repository
- Initialize git file

```
$git init 
```


- Add the files 

```
$git add .
```

- Commit at the command line

```
$git commit -m "commit"
```

- use to create a connection from local repo to server repo

```
$git remote add origin HTTPS/SSH
```
- Push code 

```
$git push origin branch
```


</details>

<br></br>

### Chapter 3. Branching, Places and GUIs

<details>
<summary>1. Five places</summary>


- The work area : it is possible to have more than one work area ( out of rader ) .
- The index (staging area) 
- The local repository : commit 
- The remote repository : pushing data 
- The stash : save files that have been fixed but not committed or lost when changing branches.

</details>

<details>
<summary>2. Branches</summary>

- Create a new branch 

```
$git branch <branch>
```

```
$git checkout -b <branch>
```

- See commits and announcements

```
$git log  --oneline
```
- Push new branches

```
$git push
```
- Combine add and commit

```
$git commit -a -m "Add the add method"
```

- Check commits

```
$git log
```

</details>

<br></br>

### Chapter 4. Merge, Pull Request and Handling Merge Conflicts

<details>
<summary>1. Merge</summary>

 Merge is the process of combining two or more branches of source code into a single branch. This allows developers to bring together changes made on separate branches and ensures that the final source code works as intended. To merge two branches, you can use the git merge command with the name of the branch to merge.

```
$git merge <branch-name>
```

</details>


<details>
<summary>2. Pull Requests</summary>

Pull Requests are a way for developers to propose changes to a codebase and have the request reviewed and merged. This allows developers to collaborate with each other and ensures that changes are properly checked out and tested before being added to the master branch. To create a Pull Request, you can use a source code hosting service like GitHub

</details>

<details>
<summary>3. Merge conflicts</summary>

1. Identify conflicting files:

```
$git merge
```

```
$git status
```

2. Open conflicting files

3. Resolve conflicts

4. Save changes

5. Thêm các thay đổi

```
$git add
```

6. Commit the changes

```
$git commit
```

7. Push the changes

```
$git push
```

</details>

<br></br>

### Chapter 5. Rebasing, Amend and Cherry-Picking

<details>
<summary>1.Rebasing</summary>

<details>
<summary>What is the rebasing?</summary>

Rebasing is the process of moving your current branch to another branch and reselecting the commits on the original branch to include them in your current branch. This process helps to merge changes across different branches and minimizes the dispersion of data in the commit history.

</details>

- Go to your current branch and run the command

```
$git rebase <branch name you want to merge into>
```

- Git will move your current branch to the branch you want to merge into and reselect the commits on the original branch to include them in your current branch.

- Once done 

```
$git log
```
</details>

<details>
<summary>2.  Amend</summary>


<details>
<summary>What is the Amend ?</summary>

Amend is a feature that allows you to modify previously created commits. It allows you to add or remove files, change commit messages, or edit previously committed changes. With this feature, you can adjust your commit history flexibly and conveniently.

</details>

- Make the changes on your file.
- Run the command to add the changes to index.

```
$git add <filename>
```

- Modify the last commit on your current branch.

```
$git commit --amend
```

- Git will open an editor where you can modify commit messages, add or remove files, or edit previously committed changes. Save and close the editor when done.

</details>

<details>
<summary>3. Cherry-Picking</summary>

<details>
<summary>What is the Cherry-Picking?</summary>
Cherry-Picking is the process of selecting commits on another branch and applying them to your current branch. This process allows you to take specific changes from one branch and move them to another branch independently. Cherry-Picking is often used when you want to apply some changes from another branch without wanting to merge that whole branch into your current branch.
</details>

- Go to your current branch and run the command: 

```
$git cherry-pick <commit code you want to apply>
```

- Review new commit history.

```
$git log
```

</details>

<br></br>

### Chapter 6. Interactive Rebasing

<details>
<summary>1. What is the Interactive Rebasing?</summary>
Interactive rebase is a feature in Git that allows you to interact with and edit existing commits on a branch. This feature is useful when you need to clean up the commit history, merge multiple commits into one, or split a commit into several smaller commits.
</details>


<details>
<summary>2. Command</summary>

```
$git rebase -i <commit>
```

> <commit> : commit hash, branch name or tag

</details>


<details>
<summary>3. Optional keywords</summary>

- Pick: Select this option to leave the commit unchanged.
- Edit: Select this option to pause rebasing after this commit, allowing you to edit the commit message, commit content, or add new changes.
- Squash: Select this option to combine this commit with the previous commit and merge the commit message together.
- Fixup: Select this option to combine this commit with the previous commit but ignore the commit message.
- Reword: Select this option to modify the commit message.

</details>

<br></br>

### Chapter 7. Workflow, Notes and Tags


<details>
<summary>1. Workflow</summary>


<details>
<summary></summary>

</details>



</details>

<details>
<summary></summary>


<details>
<summary></summary>

</details>


</details>

<details>
<summary></summary>

<details>
<summary></summary>

</details>

</details>

<br></br>

### Chapter 8. Aliases



<br></br>

### Chapter 9. Using the Log
