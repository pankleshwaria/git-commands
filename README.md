# git-commands
A list of basic git commands that you would most probably end up using.

## Lets get it started
```bash 
git config --global user.name <name-of-the-user-committing-the-changes> 
```
These settings are needed to identify the user name who is making the change to the git repo. These setting are stored in the global file. Theis info is shown in the commit log.

```bash
git config --global user.email <email-of-the-user-committing-the-changes> 
```
These settings are needed to identify the user email who is making the change to the git repo. These setting are stored in the global file. Theis info is shown in the commit log.

```bash
git config --list
```
List all config settings

```bash
git config --global --list
```
List all global config settings

```bash
git init
```
Initialize a empty git repo. If this command is run in folder containing files, git will start tracking those files.

```bash
git status
```
Shows the status of tracked files. Shows if the file is unstaged, staged, etc

```bash
git add <file-name>
```
Adds the file to staging area

```bash
git add .
```
Adds all the file in the current location to staging area

```bash
git commit -m '<commit-message>'
```
Commits the file with the message. Git will start maintaining snapshots of the file once the file is committed. There will be a commit history maintained for the file.

```bash
git commit --interactive
```
Commits the file with the message. Opens an editor to enter a detailed message. Works same like `git commit -m <commit-message>`

```bash
git log
```
Show commit history with the most recent commit on the top.

```bash
git log -2
```
Shows logs of recent 2 commits. You can display log of any number of recent commit with - <number>.

```bash
git log -stat
```
Give stats of how many lines, files are changed along with other log details.

```bash 
git show <commit-id>
```
Shows the changes commit at that commit id.

```bash
git rm <file-name>
```
Removes the file from the working tree and stage it for deletion.

```bash
git rm --cached <file-name>
```
Just removes the file from the working tree. You later need to stage the changes.

```bash
git checkout <file-name>
```
Checkout the file from remote repo to your locale repo. Be cautious doing this will loose all your changes from from the working tree and the file will be revert to same as that on remote repo.

```bash 
git diff
```
Compares file in the working tree with staging and shows the difference.

```bash 
git diff --staged
git diff --cached
```
Compares the staged/staging area file with the committed file and shows the difference.

```bash
git remote
```
List all remote repositories.

```bash
git remote -v
```
Detail list of remote repositories.

```bash
git remote show <remote-name>
```
Shows detail info of the mentioned remote.

## Contributing and Licence
This repo is only for educational purpose. Feel free to do clone, modify and share this repository.
If you find an error or have questions, feel free to write comments or raise an issue. If you want to contribute, feel free to hand in a 
pull-request.
