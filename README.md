# formssi-docs
This repos is using form keeping docs

Roy Peng:
Use git to synchronize the local repository to the github remote repository

1.Download and install git client Windows version.

2.Create a local repository folder.

3.Right-click Git Bash Here in your local repository.

4.Initialize the local repository.
<git init>
A hidden folder called git is created in the repository after execution.
Make sure there is no.git (hidden file) in the current repository before execution
  
5.Add all files in this folder to the local repository.
<git add .>
Notice there's one .  Mean Add all files in the folder to the local repository.
Before executing the command, you can add [. Gitignore] files to the directory and configure directories and files that are not committed.
  
6.Submit the file you just added to the local repository.
<git commit -m "init">
-m is followed by the content of comments, usually used to distinguish committed versions.

7.Establish a connection between the local repository and the github remote repository.
<git remote add origin https://github.com/*****/*****.git>
Origin followed by your github warehouse address.

8.Merge version, that is, pull the extra differential files from the github repository to the local repository.
<git pull origin master --allow-unrelated-histories>
Need to bring in the relatively new Git version parameter - allow - unrelated - nothing,otherwise an error [refusing to merge unrelated nothing.
Sometimes you will be asked to add comments for the merged version during this period, and then save the comments.
  
9.Synchronize the local repository to the github remote repository.
<git push -u origin master>
