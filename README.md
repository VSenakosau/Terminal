# Terminal - homework 1
## 1. Look where I am.
```
vvsen@Vadim MINGW64 ~
$ pwd
/c/Users/vvsen
```
## 2. Create a new folder
```
vvsen@Vadim MINGW64 /c/vadim/qa/HW_terminal
$ mkdir hw1
```
## 3. Go to the created folder
```
vvsen@Vadim MINGW64 /c/vadim/qa/HW_terminal
$ cd hw1
```
## 4. Create 3 new folders
```
vvsen@Vadim MINGW64 /c/vadim/qa/HW_terminal/hw1
$ mkdir folder1 folder2 folder3
```
## 5. Go to any folder
```
vvsen@Vadim MINGW64 /c/vadim/qa/HW_terminal/hw1
$ cd folder1
```
## 6. Create 5 files (3 txt, 2 json)
```
vvsen@Vadim MINGW64 /c/vadim/qa/HW_terminal/hw1/folder1
$ touch first.txt second.txt third.txt fourth.json fifth.json
```
## 7. Create 3 new folders
```
vvsen@Vadim MINGW64 /c/vadim/qa/HW_terminal/hw1/folder1
$ mkdir subfolder1 subfolder2 subfolder3
```
## 8. Show a list of the folder contents
```
vvsen@Vadim MINGW64 /c/vadim/qa/HW_terminal/hw1/folder1
$ ls
```
In response, we received:
```
fifth.json  fourth.json  subfolder1/  subfolder3/
first.txt   second.txt   subfolder2/  third.txt
```
## 9-11) Open any txt file. Write something there, any text. Save and exit.
To open a file "first.txt " we use the text editor "nano":
```
vvsen@Vadim MINGW64 /c/vadim/qa/HW_terminal/hw1/folder1
$ nano first.txt
```
Enter the following text:
```
It's my life
It's now or never
I ain't gonna live forever
I just want to live while I'm alive
(It's my life)
My heart is like an open highway
Like Frankie said I did it my way
I just wanna live while I'm alive
It's my life
```
Save changes to the file and exit:
```
press ctrl + O -> enter (save)
press ctrl + X -> enter (exit)
```
## 12. Exit the folder to the level above.
```
vvsen@Vadim MINGW64 /c/vadim/qa/HW_terminal/hw1/folder1
$ cd ..
```
Now we are in this directory:
```
vvsen@Vadim MINGW64 /c/vadim/qa/HW_terminal/hw1
```
## 13. Move any 2 files you created to any other folder.
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1/folder1
$ mv first.txt second.txt subfolder1
or
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1/folder1
$ mv first.txt second.txt /c/vadim/qa/hw_terminal/hw1
```
## 14. Copy any 2 files you created to any other folder.
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1/folder1
$ cp third.txt fourth.json subfolder2
or
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1/folder1
$ cp subfolder2/{third.txt,fourth.json} subfolder3
```
## 15. Find the file by name.
```
