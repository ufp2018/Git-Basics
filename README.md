# Git-Basics

## Helpful websites
Add more if you want. 

* [GitHub for noobs](https://www.youtube.com/results?search_query=github+for+noobs)
* [Hello World](https://guides.github.com/activities/hello-world/#repository )

## Using the web interface


1. Download the zip file (click green button).
1. Unzip and edit files on your machine.
1. Go back to the repo and click the upload file button. Upload the files you edited. 
1. Choose to commit directly to the master branch, or opt to submit a pull request and have someone else resolve conflicts.
1. If you committed directly, you might need to fix conflicts. In the web interface, you will be prompted fix conflicts. To do this, search the conflicted file for `<<<<<<<`, `=======`, or `>>>>>>>`. It will look something like this;
```
If you have questions, please
<<<<<<< HEAD
open an issue
=======
ask your question in IRC.
>>>>>>> branch-a
Decide if you want to keep it. 
```
At this point, you decide if you want to keep the old content
```
<<<<<<< HEAD
open an issue
=======
```
or the new content
```
=======
ask your question in IRC.
>>>>>>> branch-a
```
To do this just delete what you don't want, including the `<<<<<<<`, `=======`, or `>>>>>>>`. Then commit your changes. More info on merging can be found here,

* [https://help.github.com/articles/resolving-a-merge-conflict-using-the-command-line/](https://help.github.com/articles/resolving-a-merge-conflict-using-the-command-line/)

## Using terminal or GitBash

This is just a basic protocol for using git via command line. This procedure will let you keep a local version of the files on your machine. 

* clone repo to your account if not already there. You can copy the URL from the green button. (Here the `$` just means the beginning of your command line.)
``` 
	$ git clone https://github.com/ufp2018/REPO-NAME.git
```
* At this point you can edit at will. Once finished with edits, you will need to add and commit changes. Make sure you are in the repo (navigate with `cd` and `ls`). 
* You can view the status of the commits 
* Adding all new files (tells git what files to track):
``` 
	REPO-NAME$ git add .
 ```
* Commit your changes
```
	REPO-NAME$ git commit -am 'message'
```
* Pull new changes from server. At this point you might have to fix conflicts. To do this goto the conflicted file and search for the `<<<<<<<`, `=======`, or `>>>>>>>` as above. 
```
	REPO-NAME$ git pull
```
* Push your changes to server.
```
	REPO-NAME$ git pull
```





