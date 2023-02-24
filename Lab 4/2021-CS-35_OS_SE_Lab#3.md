# Task 1

---

> 1. Create a simple script which will take two command line arguments and
>   then multiply them together
> 2. Create a simple script, which will ask the user for a few pieces of
>   information then combine this into a message which is echo'd to the screen.
> 3. Now Mr. Tom suddenly lost the track of his current location. Help him find
>   his location.
> 4. He wants the list of all files present on home directory.
> 5. Display the current time.
> 6. He is done with the task and he is happy with your work. He want to
>   display a thankyou message.

---

NOTE: **USE nano instead of gedit**

1. Create a file name *Script.sh* using **touch script.sh** and now edit file using **gedit script.sh** and type the following code

   ```
   #!/bin/bash
   product=$(($1*$2));
   echo "$product";
   ```

   Then run the following  **bash script.sh 3 2**

   ```
   //6(3+2)
   ```

   ​

2. Create a file name *Script2.sh* using **touch script2.sh** and now edit file using **gedit script2.sh** and type the following code

   ```
   #! /bin/bash
   echo "Enter name"
   read name
   echo "Enter marks"
   read marks
   echo "Enter city"
   read city
   echo "$name from $city got $marks";
   ```

   Then run the following  **bash script2.sh**

   ![](\1.png)

   ​

3. Type **pwd** and hit enter this will result in present working directory

4. **cd ~** will take you to home and **tree** or **ls -l** to list all files.

   ```
   //change the current document to 
   ```

   ​

5. Type **date**  and hit enter will result in current date.

6. **echo "Thank You Muhammad Subhan"**

# Task 2

------

> 1. Write a simple shell script that uses arithmetic operators (+, -,*) using
>    double parenthesis with printing your own roll # with the results of
>    operations.
> 2. Write a simple shell script that uses all relational operators with printing
>   your own roll # with the results of operations.

1. Create a file name *Script3.sh* using **touch script3.sh** and now edit file using **gedit script3.sh** and type the following code

   ```
   /bin/bash
   echo "Write yor roll no"
   read roll_no
   echo "$((roll_no*roll_no))is product of $roll_no";
   echo "$((roll_no+roll_no)) is sum of Sroll_no";
   echo "$((2*roll _ no-roll_no)) is difference of 2*roll_no*roll _ no $roll_no" ; 
   ```

   ![](\2.png)

Create a file name *Script3.sh* using **touch script3.sh** and now edit file using **gedit script3.sh** and type the following code:

```
/bin/bash
echo "Write yor roll no"
read roll_no
if [$roll -ne 35]
then 
	echo "$roll is not equal to 35";
if [$roll -eq 35]
then 
	echo "$roll is  equal to 35";
if [$roll -gt 35]
then 
	echo "$roll is  greater than  35";
if [$roll -lt 35]
then 
	echo "$roll is  less than to 35";
	
```

![](\3.png)

This will output if the  compare roll number with 35