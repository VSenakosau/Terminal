# Terminal - homework 2
## 1. Make a dir_1 folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2
$ mkdir dir_1
```
## 2. Go to the dir_1 folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2
$ cd dir_1
```
## 3. Create the inner_dir_1 folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ mkdir inner_dir_1
```
## 4. See where you are
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ pwd
```
Response:
```
/C/Vadim/QA/HW_terminal/hw2/dir_1
```
## 5. While in the dir_1 folder, create an empty text file tf_1.txt
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ touch tf_1.txt
```
## 6. While in the dir_1 folder, use the cat command to create a text file tf_2.txt with the following lines:
- the first 1
- the second 2
- the third 3
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ cat > tf_2.txt
- the first 1
- the second 2
- the third 3
```
After entering the information in `tf_2.txt` press `Ctrl+D` to save and exit  
## 7. Go to the inner_dir_1 folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ cd inner_dir_1
```
## 8. Use the `cat` command to create a text file tf_3.txt with any strings
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1/inner_dir_1
$ cat > tf_3.txt
It`s a beautiful day
The sun is shining
I feel good
```
After entering the information in `tf_3.txt` press `Ctrl+D` to save and exit  
## 9. Via command `cat` add to a text file tf_3.txt the line "the second 2"
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1/inner_dir_1
$ cat>> tf_3.txt
the second
```
Using the `>>` operator with command `cat` allows you to append content to an existing file  
## 10. Via command `cat` add to a text file tf_3.txt the line "the sec 2"
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1/inner_dir_1
$ cat >> tf_3.txt
the sec 2
```
After entering the information in `tf_3.txt` press `Ctrl+D` to save and exit  
## 11. Via command `cat` add to a text file tf_2.txt the line "the sec 3"
Since my current directory is inner_dir_1 (level below), I have to show the path to the file tf_2.txt
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1/inner_dir_1
$ cat >> /C/Vadim/QA/HW_terminal/hw2/dir_1/tf_2.txt
the sec 3
```
After entering the information in `tf_2.txt` press `Ctrl+D` to save and exit  
## 12. Via command `cat` add to a text file tf_3.txt the line "the SeCoNd 2"
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1/inner_dir_1
$ cat >> tf_3.txt
the SeCoNd 2
```
After entering the information in `tf_3.txt` press `Ctrl+D` to save and exit 
## 13. Via command `cat` add to a text file tf_2.txt the line "the seConD 2"
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1/inner_dir_1
$ cat >> /C/Vadim/QA/HW_terminal/hw2/dir_1/tf_2.txt
the seConD 2
```
After entering the information in `tf_2.txt` press `Ctrl+D` to save and exit  
## 14. Make a text file tf_4.txt with 15 lines
You can manually enter 15 lines. But we use the `seq` command to generate a sequence of numbers. It takes one or two arguments that define the beginning and end of the sequence.
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1/inner_dir_1
$ seq 1 15 > tf_4.txt
```
## 15. Make a text file tF_5.txt with 13 lines
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1/inner_dir_1
$ seq 1 13 > tF_5.txt
```
## 16. Display a list of all files in the folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1/inner_dir_1
$ ls
```
Response:
```
tF_5.txt  tf_3.txt  tf_4.txt
```
## 17. Exit from the inner_dir_1 folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1/inner_dir_1
$ cd ..
```
## 18. Output the contents of file tf_3.txt to the terminal
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ cat inner_dir_1/tf_3.txt
```
Response:
```
It`s a beautiful day
The sun is shining
I feel good
the second
the sec 2
the SeCoNd 2
```
## 19. Find the file tf_4.txt and the path to it
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ find ./ -name tf_4.txt
```
Response:
```
./inner_dir_1/tf_4.txt
```
## 20. Clear the file tf_4.txt of its contents without deleting the file itself.  
We can use the `>` redirection operator alone to clear the contents of a file without deleting the file itself.  
Using `>` without any preceding command will truncate the file "tf_4.txt" to zero length, effectively clearing its contents while preserving the file itself.
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ > inner_dir_1/tf_4.txt
```
## 21. Find the path to files that have "tf" in their names
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ find ./ -name "*tf*"
```
Response:
```
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_4.txt
./tf_1.txt
./tf_2.txt
```
In the context of the find command, the asterisk `*` is a wildcard character that represents any number of characters.
By using `./` as the starting point, the search is limited to the current directory.
## 22. Find the path to files that have "tf" in the name and letters in any case
The `-name` parameter searches for file names without case
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ find ./ -iname "*tf*"
```
Response:
```
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_4.txt
./inner_dir_1/tF_5.txt
./tf_1.txt
./tf_2.txt
```
## 23. Find lines in files where there is a combination of letters "sec" in the current folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ grep "sec" *
```
Response:
```
grep: inner_dir_1: Is a directory
tf_2.txt:- the second 2
tf_2.txt:the sec 3
```
grep "sec" `*` searches only within the files in the current directory, excluding subdirectories
## 24. Find lines in files where there is a combination of letters "sec" in any case in the current folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ grep -i "sec" *
```
Response:
```
grep: inner_dir_1: Is a directory
tf_2.txt:- the second 2
tf_2.txt:the sec 3
tf_2.txt:the seConD 2
```
The `-i` option instructs grep to ignore the case of the letters when performing the search.
## 25. Find lines in files where there is only a combination of letters "sec" in the current folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ grep -w "sec" *
```
Response:
```
grep: inner_dir_1: Is a directory
tf_2.txt:the sec 3
```
The `-w`option ensures that only lines with "sec" as a standalone word are matched, excluding cases where "sec" is part of a larger word.
## 26. Find lines in files where there is only a combination of letters "sec" in any case in the current folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ grep -wi "sec" *
```
Response:
```
grep: inner_dir_1: Is a directory
tf_2.txt:the sec 3
```
## 27. Find lines in files where there is a combination of letters "second" in the current folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ grep "second" *
```
Response:
```
grep: inner_dir_1: Is a directory
tf_2.txt:- the second 2
```
## 28. Find lines in files where there is a combination of letters "second" in any case in the current folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ grep -i "second" *
```
Response:
```
grep: inner_dir_1: Is a directory
tf_2.txt:- the second 2
tf_2.txt:the seConD 2
```
## 29. Find lines in files where there is a combination of letters "second" in all folders below the level
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ grep -r "second"
```
Response:
```
inner_dir_1/tf_3.txt:the second
tf_2.txt:- the second 2
```
## 30. Find only the path and file name with the combination of the letters "second" in the current folder
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ grep -l "second" *
```
Response:
```
grep: inner_dir_1: Is a directory
tf_2.txt
```
or
```
vvsen@Vadim MINGW64 /C/Vadim/QA/HW_terminal/hw2/dir_1
$ grep -ls "second" *
```
Response:
```
tf_2.txt
```
`-l` option: This option instructs grep to display only the filenames of the matching files, rather than showing the matching lines.  
The directory inner_dir_1 is listed as an error message when using grep `-l "second" *` because it is treated as a file, and grep attempts to search within it.  
The `-s` option suppresses the error message for the directory inner_dir_1.  
