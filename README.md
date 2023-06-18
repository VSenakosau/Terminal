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
`tail -f` command is used to output the last part of a file and the `-f` option enables "follow mode" to monitor the file continuously for new updates.   
`|` is used to redirect the output of the preceding command as the input to the following command.
`grep -i "knowledge"`  is used to search for specific patterns or text within the input. The `-i` option is used to perform a case-insensitive search.   
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
## 19. View the contents of a long file (less command)
We need a file with a long text. Use www.lipsum.com to generate a text of 3000 words and save it to a file second.txt
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1/folder2
$ less second.txt
```
Press the `Enter` key to scroll forward one line  
Press the `Spacebar` to scroll forward one page at a time  
Press the `b` to scroll backward one page  
Press the `d` key to scroll down half a page  
Press the `u` to scroll up half a page  
Press the `g` to jump to the beginning of the file  
Press the `G` to jump to the end of the file  
Use `-N` to display line numbers  
Use `/Lorem` to find all the words "Lorem" in this file  
You can search forward `/` or backward `?` and navigate to the next `n` or previous `N` 
Press the `q` to exit  
## 20. Show date and time (current)  
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1/folder2
$ date
```
The response:
```
Sun May 21 16:55:56     2023
```
## 21. Send an http request to the server http://162.55.220.72:5005/terminal-hw-request
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal/hw1/folder2
$ curl http://162.55.220.72:5005/terminal-hw-request
```
The response:
```
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --100   232  100   232    0     0   2275      0 --:--:-- --:--:-- --:--:--  2297<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2 Final//EN">
<title>404 Not Found</title>
<h1>Not Found</h1>
<p>The requested URL was not found on the server. If you entered the URL manually please check your spelling and try again.</p>
```
The response received indicates that the server returned a 404 Not Found error.  
## 22. Write a script that will automatically execute the items 3, 4, 5, 6, 7, 8, 13
Creating a file myscript.sh
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal
$ touch myscript.sh
```
Opening the file myscript.sh through the `nano` editor    
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal
$ nano myscript.sh
```
Enter the following information:  
```
#!/bin/bash  
cd C:\\Vadim\\qa\\hw_terminal\\hw1  
mkdir folder4 folder5 folder6  
cd folder4  
touch first.txt second.txt third.txt fourth.json fifth.json  
mkdir subfolder4 subfolder5 subfolder6  
ls  
mv first.txt second.txt subfolder4  
echo "You did it, you are great"  
```
Press  
ctrl+O -> Enter  
ctrl+X  
Let's make this file executable, otherwise, if you try to run it, you will encounter the Permission denied error  
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal
$ chmod +x myscript.sh
```
Now we can execute the script myscript.sh
```
vvsen@Vadim MINGW64 /c/vadim/qa/hw_terminal
$ ./myscript.sh
```
The response:
```
fifth.json  fourth.json  subfolder4  subfolder6
first.txt   second.txt   subfolder5  third.txt
You did it, you are great
```
