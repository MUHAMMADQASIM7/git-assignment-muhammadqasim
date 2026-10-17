
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
