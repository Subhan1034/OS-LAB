# Task 1

---

> You are required to help a new Ubuntu user in performing Ubuntu commands.
> Mr. Tom is new Ubuntu user. He want guidance regarding basic Ubuntu utilities to
> perform following tasks:
>
> 1. Create a file named “19f-XXXX.txt”. File must contain at least 10 lines.
> 2. Create another file named “your name.txt”. File must contain at least 10 lines.
> 3. Merge the data of both files.
> 4. Redirect the output to a new file.
> 5. Display the first two lines of first file.
> 6. Display the last two lines of second file.
> 7. Finds the string (your roll#) from the first file.
> 8. Grant the execute permission of the second file to the group.
> 9. Remove the write permission for the owner.
>   10.Now Mr. Tom suddenly lost the track of his current location. Help him find his
>   location.
>   11.He wants the list of all files present on Desktop directory.
>   12.Now he wanted to create a folder of his personal files and pictures named as
>   your roll#.
>   13.Display the current time.
>   14.He is done with the task and he is happy with your work. He want to display a
>   thankyou message.

---

1. Open Terminal by pressing **Ctrl+Alt+T** and type **touch 19f-XXXX.txt ** and add text using **gedit 19f-XXXX.txt**.
2. Type **Subhan.txt ** and add text using **gedit Subhan.txt**;
3. Type **cat 19f-XXXX.txt >> Subhan.txt**  and add both file will be merged.
4. **cat 19f-XXXX.txt Subhan.txt  >> newfile.txt**  and add both file will be redirected to newfile.txt.
5.  **head -2 19f-XXXX.txt ** will display first two lines
6.  **head -2 Subhan.txt** will display first two lines
7. **grep -r "35" Subhan.txt**
8. **chmod g+e Subhan.exe**
9. **chmod o-w Subhan.exe**
10. **pwd**
11. **cd ~**
12. **ls -l** or **tree**
13. **date**
14. **echo Thank You**

# Task 2

------

> 1. Create a file named “19f-XXXX_OS-lab_rules.txt” using linux commands. .
> 2. You want to set the rights of created file to this (- rwx r-x r--). For these rights, you are required to convert the given rights in numeric format using binary number system procedure covered in lecture. Show complete working.
> 3. Now use the derived number to change the permission of a file using chmod command.
> 4. Append the output of ls command to created file.

1. Open Terminal using **Ctrl+Alt+T** and type **touch 19f-XXXX_OS-lab_rules.txt** 
2. **chmod 754 19f-XXXX_OS-lab_rules.txt**