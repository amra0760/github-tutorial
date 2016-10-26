# GitHub Tutorial

##### _by Amr Almaz_

---
## Git vs. GitHub
**Git:** keeps snapshots of code so if you have an error or a mistake you can see where you messed up. Git doesn't require Github in order for it to work. Git can work on many other websites such as cloud9.  
**Github:** is the cloud or the website that stores git and made git. Github requires git in order to run because it is the website that launched git.  

---
## Initial Setup
#### How to Make a Github Account 
1. First you go to [Github.com](github.com)  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/Screen%20Shot%202016-10-24%20at%208.34.34%20AM.png?_c9_id=livepreview0&_c9_host=https://ide.c9.io)    
2. Then you set a username and password (HSTAT students use your hstat email and password) ***If you recieved a error message just ignore it***  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/Github%20Account.PNG?_c9_id=livepreview20&_c9_host=https://ide.c9.io) ![What it looks like for hstat students](https://preview.c9users.io/amra0760/github-learning/github-tutorial/Github%20Account%20(HSTAT).PNG?_c9_id=livepreview5&_c9_host=https://ide.c9.io)  
3. Check your email for verfication from github  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/Email%20Verification.PNG?_c9_id=livepreview6&_c9_host=https://ide.c9.io)  
4. Open and click verify!  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/Verfiy%20Button.PNG)
5. Then go back to github.com and click on "Free Account"
6. To finalize making your github account click on "Finish Sign Up"

#### How to Connect your Github Account to Cloud 9  
1. First you go to [c9.io](c9.io)  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/go%20to%20c9.PNG?_c9_id=livepreview14&_c9_host=https://ide.c9.io)  
2. Then you click on the Octocat  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/github%20sign%20in.PNG?_c9_id=livepreview15&_c9_host=https://ide.c9.io)  
3. Then you sign in with your username that you made earlier on github  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/github%20sign%20in%202.PNG?_c9_id=livepreview16&_c9_host=https://ide.c9.io)  
4. Then you click on the gear icon in the top right corner of the page  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/gear%20icon.PNG?_c9_id=livepreview17&_c9_host=https://ide.c9.io)  
5. Then you click on connected services  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/connected%20services.PNG?_c9_id=livepreview18&_c9_host=https://ide.c9.io)  
6. Then you click on connect next to github  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/connect%20to%20github.PNG?_c9_id=livepreview19&_c9_host=https://ide.c9.io)  
7. Now you're connected!

#### How to Create an SSH key between Github & Cloud
1. Go to [Github.com](github.com)  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/Screen%20Shot%202016-10-24%20at%208.34.34%20AM.png?_c9_id=livepreview0&_c9_host=https://ide.c9.io)    
2. Sign in
3. Click on your profile icon on the top right
4. Then click on settings
5. Go to the left sidebar and click on "SSH and GPG keys"
6. Click on "New SSH key"
7. Make the title _cloud9_
8. Now go back to cloud9
9. Click on the gear icon in the top right corner
10. Click on "SSH Keys"
11. Copy the SSH Key given
12. Then go back to github.com and paste the SSH key
13. Then add the SSH Key
14. Now go back to cloud9 again and open "github-learning IDE"
15. Then type in `ssh -T git@github.com`
16. Finally a message should come up that say that it worked but you dont have shell access
17. CONGRATUTLATIONS YOU HAVE NOW MADE A SSH KEY BETWEEN Github and Cloud9!


---
## Repository Setup
#### How To Make a Repository in c9
1. First open up [c9.io](c9.io)  
![](https://preview.c9users.io/amra0760/github-learning/github-tutorial/go%20to%20c9.PNG?_c9_id=livepreview14&_c9_host=https://ide.c9.io)  
2. Then make sure that you're in the workspace directory (if your not sure then type in `cd ~/workspace`)  
3. Now to make any type of directory you have to use the syntax: `mkdir (DirectoryName)`. Name the directory whatever you like but try to keep it short and simple.  
4. **Now this step is very crucial. You have to get in to your directory before you intialize it**. You do this by typing `cd (DirectoryName)`.  
5. Following that you can use `git status` to track the status of your directory and you will see an error coming up that says: "`fatal: Not a git repository (or any of the parent directories): .git`"".  
6. Now what you want to do is intialize your directory and you do this by simply typing `git init`. Now you should see your directory's name with the word "master" in parenthesis nex to it. That means that you were succesfull in intializing your directory and have now made it a "repo". (If you want to double check use `git status` and it should say `on branch master`)  

#### How To Make a Repository in github  

#### How To Make a file in c9  
1. Now that you have a repo you probably want to put files inisde of it. The syntax for it is `touch (filename)`.  
2. If you have already typed git status you should know that the next step is that you need to use `git add` to track the repo and that is your next step
3. Now you commit using `commit -m "(message)"

---
## Workflow & Commands  
#### Here are some commands that you should familiarize yourself with while using git:  
1. `git status` - This is one of the most helpful commands there are out there. Feel free to use this command whenever and wherever you want because it only checks the condition or the status you are in right now.    
2. `git init` - This, when used inside a directory, will intialize it for version control which means that it will make the tools ready to get utilized.  
3. `git add` - This adds your file to the staging area
4. `git commit -m` - This command will take a snapshot of the all the files on the staging area so far and will also label it with a message. The point of the message is so that you can see what you have added or deleted or changed.  
5. `git push` - This will push or save your changes/commits of your local repo up to the remote repo/orgin master.  
6. `git diff` - This will check the difference between your last commit and your previous commits. The stuff that you took out will have a (-) sign next to it and the things that you have inserted will have a (+) next to it.  
7. `git log` - This previews all the commits you have commited so far.  
8. `rm -rf .git` - This can delete a repo, directory, or file with whatevers is in it. This is also used to unstage a file.
