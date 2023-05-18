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

### [Chapter 10. Important Git Commands and Metadata]()

### [Chapter 11. Finding a Broken Commit: Bisect and Blame]()

### [Chapter 12. Fixing Mistakes]()

### [Chapter 13. Next Steps]()

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

> '<commit>' : commit hash, branch name or tag

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
<summary>What is the workflow?</summary>
Workflow is the process of working with branches, commits and merges
</details>



</details>


<details>
<summary>2. Notes</summary>

<details>
<summary>What is the notes?</summary>
 A node is an object that stores information about a specific commit. Each commit in Git has a unique node, called a "SHA-1 hash", which is a 40-character string used to identify and determine the commit.
</details>

- Viewing information about a specific commit:

```
$git show <commit-hash>
```

- Viewing information about the entire history of a repository:

```
$git log
```

- Viewing information about the history of a specific branch:

```
$git log <branch-name>
```

- Viewing information about the history of a specific file:

```
$git log <file-name>
```

- Viewing information about the history of a specific folder:

```
$git log <folder-name>
```

- Searching for commits based on the content of the commit message or changes:

```
$git log --grep="<search-term>"
```


</details>

<details>
<summary>3. Tags</summary>

<details>
<summary>What is the tags?</summary>
"Tags" is one of the important features of Git, allowing you to mark specific commits as released versions of your software or project. A tag is simply a label (name) attached to a specific commit in the history of your repository.
</details>

- Creating a new tag:

```
$git tag <tag-name>
```

- Marking a specific commit as a version:

```
$git tag <tag-name> <commit-hash>
```

- Viewing a list of existing tags:

```
$git tag
```

-Viewing the details of a tag:

```
$git show <tag-name>
```

- Deleting a tag:

```
$git tag -d <tag-name>
```

- Pushing a tag to a remote repository:

```
$git push origin <tag-name>
```

- Pushing all tags to a remote repository:

```
$git push --tags
```

</details>

<br></br>

### Chapter 8. Aliases

<details>
<summary>1. Create alias</summary>


```
$ git config --global alias.<alias-name> '<git-command>'
```

> '<git-command>' Git command that you want to minify to alias.

</details>



<details>
<summary>Create the st alias</summary>

```
$git config --global alias.st status
``` 

</details>



<details>
<summary>Create a branch and 
check it out</summary>

```
$git config --global alias.bc checkout -b 
$git config --global alias.cb checkout -b 
``` 

> The important thing to notice here is that your alias can take one or more flags. 

</details>



<details>
<summary>A lot commits everything and waits for a message</summary>

```
$git config --global alias.cam commit -a -m
``` 

</details>

<details>
<summary>Commits everything along with the message you give it</summary>

```
$git cam  "Here is you message"
``` 

</details>


<details>
<summary>Offers me an alternative to log --oneline that gives much more information</summary>

```
$git config –global alias.lg log --graph --pretty=format:'%Cred%h%Creset 
-%C(yellow)%d%Creset %s %Cgreen(%cr) %C(yellow)<%an>%Creset' --abbrev-commit
``` 

</details>


<details>
<summary>Opens the global configuration file in your editor</summary>

```
$git config --edit --global
``` 

- Note :
>  You can add aliases directly here if you like.
>  If you are going to use more than one flag

```
$git config --global alias.nx "log --name-only --oneline"
```

</details>

<br></br>

### Chapter 9. Using the Log

<details>
<summary>Log at the command line</summary>

```
$git log --oneline
``` 

</details>

<details>
<summary>Which files changed?</summary>

```
$git log --name-only
``` 

</details>

<details>
<summary>Summary</summary>

The log can show you when each commit was created, who created it, and other useful information about the commit, such as what changed in each file. You have great control over what is displayed

</details>

<br></br>

### Chapter 10. Important Git Commands and Metadata

#### STASH


<details>
<summary>What is Stash ?</summary>

- Is a place where you can hold (stash) files you've modified but not yet committed


```
$git push --mirror
```

>  Copy the entire content of a Git repository to another repository, including branches, tags, and commit history.

</details>


<details>
<summary>Command</summary>


```
$git stash 
```

```
$git stash list
```
> show list stash create before

```
$git stash show
```

> Show the changes stored in the stash

</details>


#### CLEAN 

Get rid of it

<details>
<summary>Command</summary>

```
$git clean
```
> Untracked files are gone never to be seen again.


- To actually clean, Git requires that you tell it you really mean it by using the -f (force) flag : 

```
$git clean -f
```

</details>



#### METADATA

<details>
<summary>Using show to see metadata</summary>

```
$git show -s HEAD --format='%an <%ae> %h %d'
```

- git show—the show command.
- -s—silent (or quiet), which suppresses the difference output (try the 
command without it to see).
- HEAD tells show which commit you are interested in.
- %an is the author's name.
- %ae is the author's email address
- %h is the abbreviated commit hash 
- %d information about the current branch's position

</details>


<br></br>

### Chapter 11. Finding a Broken Commit: Bisect and Blame
#### BISECT


<details>
<summary>Start the search process</summary>

```
$git bisect start
```

-  Then, you need to specify the current last bad commit with the command :

```
$git bisect bad
```

- Next, you need to specify a previous commit that you know for sure is working properly with the command :

```
$git bisect good
```

</details>


#### BLAME

1. File history search

- To search for information about the commit you want to find the history of that file.

<details>
<summary>git log</summary>

- This command displays the history of commits and allows you to view information about different commits.


</details>

<details>
<summary>git branch</summary>

- This command displays a list of branches in Git's repository.

</details>

<details>
<summary>git show</summary>

- This command displays information about a specific commit.

</details>


<details>
<summary>git diff</summary>

- This command displays the difference between two commits or between two versions of the same file.


</details>

<details>
<summary>git rev-parse</summary>


- outputs the full SHA-1 hash of the current commit :

```
$git rev-parse HEAD
```

- outputs the abbreviated SHA-1 hash of the current commit :

```
$git rev-parse --short HEAD
```

- outputs the full SHA-1 hash of the tag named "v1.0.0" :

```
$git rev-parse v1.0.0
```

-  outputs the symbolic name of the current branch :

```
$git rev-parse --symbolic-full-name HEAD
```

</details>

2. Ignore whitespace changes when searching history :

```
$git blame -w
```

3. Displays the history of a file and indicates who each line was changed by:

```
$git blame -w -M3
```


<br></br>


### Chapter 12. Fixing Mistakes



<details>
<summary>Amend the last commit</summary>

- Add changes to the previous commit
- Edit the commit message and add any additional changes.
```
$git commit --amend
```

- If you don't want to edit the message when you add the files, enter:

```
$git commit --amend --no-edit
```

</details>

<details>
<summary>Undo a commit</summary>

- Creates a new commit that undoes the changes made in a previous commit.

```
$git revert
```

</details>


<details>
<summary>Reset to a previous commit</summary>

- Go back to a previous commit and discard any changes made since then

```
$git reset
```
- This will remove any commits made after the specified commit and reset the branch to that commit.

</details>


<summary>Branch name change</summary>


```
$git branch -m <currentName> <desiredName>
```

</details>

<br></br>

### Chapter 13. Next Steps

1. Creating a new branch: Use the git branch command to create a new branch for your work. You can then use git checkout to switch to that branch.

2. Making changes: Make changes to your files as needed. You can use git add to stage changes for commit.

3. Committing changes: Use git commit to commit your changes to the current branch.

4. Pushing changes: Use git push to push your changes to a remote repository.

5. Pulling changes: Use git pull to pull changes from a remote repository into your local repository.

6. Merging changes: Use git merge to merge changes from one branch into another.

7. Resolving conflicts: If there are conflicts between different versions of a file, use git mergetool to resolve them.

8. Reverting changes: Use git revert to undo changes made in a previous commit.