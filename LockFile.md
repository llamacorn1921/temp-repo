# Lock File
A lock file (for the terminal) is a file that either locks the entire folder, or a number of folders and files in said folder. \
This is used when someone wants to tell the terminal that this folder, or the contents listed in the lock file, shall not be moved or deleted. \
A lock file is named like this: `.terminal.lock`
## Why?
Well, Instead of having to modify permissions on the folder, or the files, you can just create a lock file. \
This makes the Terminal easier to remove without messing up your entire file system.

## How?
Very simple actually. \
The terminal does all the hard work, you just have to use the features that the terminal kindly provides. \
The BuiltInPackage, a package with all base commands and howtos, will have a few commands on how to interact with lock files. \



## Can we have an example?
Sure! \
This is what one looks like when the lock file is for the entire folder, contents and all:
```





```
`but it's empty?`   Exactly! \
The terminal will read the file, and if it's empty, it will lock the entire folder. \
If you want to lock a specific file or folder, you can list them in the lock file. \
```
super-secret-folder/
super-secret-file.txt
```
This will lock the folder `super-secret-folder` and the file `super-secret-file.txt`\
Just name the folder name or file to lock it. Simple as that. \

...but what if I have tons of files named similarly? \
It can handle those too!
```
super-secret-image-[1-100].png
super-secret-***.txt
image.***
image.[jpg|png|gif]
```
`super-secret-image-[1-100].png` will lock all images from 1 to 100. \
`super-secret-***.txt` will lock all files that start with `super-secret-` and end with `.txt` \
`image.***` will lock all files that start with `image.` and have format \
`image.[jpg|png|gif]` will lock all files that start with `image.` and end with `.jpg`, `.png` or `.gif` \