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
Thank you for all the Hours you spend,
A ttention you give,
Needs that you tend,
Knowledge you pass on,
Your special touch,
Offering guidance,
Undaunted by much,
Time you spend planning,
Efforts you make,
Angles to learning.
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
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1
$ mv folder1/first.txt folder1/second.txt folder2
```
## 14. Copy any 2 files you created to any other folder.
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1
$ cp folder1/third.txt folder1/fourth.json folder3
```
## 15. Find the file by name.
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1
$ find . -name first.txt
```
In response, we received:
```
./folder2/first.txt
```
## 16. View the content in real time (grep command).
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1
$ tail -f folder2/first.txt | grep -i "knowledge"
```
In response, we received:
```
Knowledge you pass on,
```
Open the "first.txt" file via the web interface and add the next line:
```
Thank you for the knowledge!
```
Then ```press``` Enter and ```Ctrl+S```
As a result, we see the added line with the keyword in the console:
```
Knowledge you pass on,
Thank you for the knowledge!
```
To exit the command, press Ctrl + C
## 17. Show the first few lines from a text file.
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1
$ head ./folder2/first.txt
```
In response, we received:
```
Thank you for all the Hours you spend,
Attention you give,
Needs that you tend,
Knowledge you pass on,
Your special touch,
Offering guidance,
Undaunted by much,
Time you spend planning,
Efforts you make,
Angles to learning.
```
If you want to specify a certain number of lines, use "-n".
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1
$ head -n 4 ./folder2/first.txt
```
In response, we received:
```
Thank you for all the Hours you spend,
Attention you give,
Needs that you tend,
Knowledge you pass on,
```
## 18. Show the last few lines of a text file.
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1
$ tail ./folder2/first.txt
```
In response, we received:
```
Attention you give,
Needs that you tend,
Knowledge you pass on,
Your special touch,
Offering guidance,
Undaunted by much,
Time you spend planning,
Efforts you make,
Angles to learning.
Thank you for the knowledge!
```
If you want to specify a certain number of lines, use "-n".
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1
$ tail -n 5 ./folder2/first.txt
```
In response, we received:
```
Undaunted by much,
Time you spend planning,
Efforts you make,
Angles to learning.
Thank you for the knowledge!
```
## 19. 
