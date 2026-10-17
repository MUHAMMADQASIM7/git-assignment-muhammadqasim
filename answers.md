
# Git Assignment — Answers


## Q1. T erminal basics (2 marks each = 6 marks)
### 1. What is a terminal? How is it different from clicking through folders in a file explorer?
### Anwser: Terminal is a interface where you can perform task by command . For example if you want to make a folder you go in file explorer and create it manualy but in terminal u just use mkdir command to make it.

### 2. Write the terminal command to: (a) list all files including hidden ones, (b) create a folder called project, (c) move into that folder .
### Anwser: 
### a) "ls -a" is the command for list all files with hidden one.
### b) "mkdir project" is the command to make folder called project.
### c) "cd project" is the command to move into that folder.

### 3. What does the cd .. command do? What about cd ~?
### Anwser: cd .. commad is use to get into parent folder 
### Anwser: cd ~ commad is use to get to the home folder 

## Q2. Version control concepts (2 marks each = 8 marks)
### 4. Explain what version control is in your own words. Give one real-world analogy (not Google Docs — pick your own).
### Awnser: Version control is a system where we can track the changes of a file .So we can see the old versions and go back to them if needed. Its like You are writting a book and u have different version of draft and in each draft changes thing and remove some and edit some and u can always go back and see your old draft as your old version of book and .
### 5. What is the difference between Git and GitHub? Can you use Git without GitHub?
### Awnser: Git is tool that is use to make changes in your repo and Github is a platform that is use to manage the repos
### 6. Name three features GitHub provides that Git alone does not.
### Anwser: Store your project in cloud , work togethere in project , can mange your project changes.
### 7. What is a repository? What is the difference between a local repository and a remote repository?
### Anwser: Repository is a place where your project and its changes save, Local repository save on your local device, remote repository is like repo saved on cloud like Github platform where u can share and work on it with multiple people.
## Q3. Git internals (3 marks each = 6 marks)
### 8. Explain what HEAD means in Git. What happens to HEAD when you switch branches?
### Anwser: Head is the position u are curently in git like the lastest commit . When u changes branches your Head move to the new branch
### 9. What is a .gitignore file? Write a .gitignore that ignores: all .log files, a folder called node_modules/, and any file ending in .env.
### Anwser: .gitignore file is use to tell git to ignore which files and folder
*.log 
<br>
node_modules
<br>
*.env


### Why did we commit A+B separately from C? When would you want to split commits this way?
### Anwser: Because A+B might have a whole task or feature and C have seperate task or feature so we do seperate commit for each task or feature so we can understand those changes and dont mix them up.
### What would happen if you made a local commit first WITHOUT pulling? What command helps you check?
### Anwser: It can cause a merge conflict and git status is the command that helps u check it.
### Did this merge create a merge commit or was it a fast-forward? How can you tell?
### Anwser: Its a fast-forward because we can see there is no merge commit in git log --oneline --graph --all command 
### Why did this conflict happen? (Reference the rule: same file, same line)
### Anwser: When there is two branches that have changes in the same files same line its gonna cause a merge conflict
### Would there have been a conflict if the two branches edited different lines of team.txt?
### Anwser: No
### Would there have been a conflict if one branch edited team.txt and the other edited about.md?
### Anwser: No
### What is the purpose of a pull request? Why not just merge directly?
### Anwser: To check if there is a problem with code before merging into main.
### Name two things a reviewer should check in a pull request.
### Awnser: CHeck if the code works fine and there is no bug and error
### What is the difference between a merge commit and a fast-forward merge?
### Anwser: When we do merge commit there will be a commit that show the merge between branches in fast-forward it will merge without making any commit

# Part 5 — Merge Conflict Scenarios

### Scenario A. Ahmed creates a branch and changes line 10 of index.html. Sara creates a different branch and changes line 1 of the same index.html. Both merge into main. Will there be a conflict? Why or why not?
### Anwser: No Because conflict cause by same file same line change.
### Scenario B. Ali edits style.css on his branch. Fatima edits app.js on her branch. Both merge into main. Will there be a conflict? Why or why not?
### Anwser: No Because conflict cause by same file same line change.
### Scenario C. Dev A changes line 5 of config.py to DEBUG = True. Dev B changes line 5 of config.py to DEBUG = False. Both merge into main. Will there be a conflict? If yes, show exactly what the conflict markers would look like in the file.
### Anwser: Yes
#### <<<<<<< HEAD
#### DEBUG = True
#### =======
#### DEBUG = False
#### >>>>>>> feature-branch


### Scenario D. You run git merge feature/new-ui and see this output:vAuto-merging index.html <br> CONFLICT (content): Merge conflict in index.html <br> Automatic merge failed; fix conflicts and then commit the result. <br> Write out the exact steps (commands included) you would take to resolve this conflict and finish the merge.
### Anwser: First i would resolve the conflit by keeping both or keeping incoming or current depend on changes. Then after resolve i commit the merge resolve with commit msg on which file ot was done.
### Scenario E. Y our teammate says:<br>"I always do git pull before I start working every morning.<br>" Is this a good practice? Explain why or why not, and what could go wrong if they skip it.
### Anwser: Its a good practice because it prevents merge conflict on the merge. If we dont git pull we will be working on old version where code is not updated to the latest repo changes that is updated by others. when u create merge request it might cause merge conflicts .