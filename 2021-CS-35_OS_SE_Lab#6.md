

#Lab 6

---

> 1. Create a Bash script to find the most occurring element in an array of integers.
> 2. Create a Bash script to find the largest element of a given array of integers.
> 3. Create a Bash script to separate 0s and 1s from a given array of values 0 and 1.
> 4. Create a Bash script to find the first repeating element in an array of integers.

####Create a Bash script to find the most occurring element in an array of integers.

1. Create a file named `touch Task1.sh.` 

   *This command creates a new empty file with the specified name. 

   ​				The syntax is **touch *newfilename****

2. Open file in nano using `nano Task1.sh`

   *This command opens the file in the nano text editor, which allows you to write and edit the Bash script.* Save and exit the file by pressing "Ctrl-X", then "Y", and then "Enter".

3. Write the code provided below:

```
#!/bin/bash
declare -a arr
arr=( 1 1 1 1 2 3 4 5 6 7 8 9 10 1 3 5 8 9 4 1 )
declare -a  element
declare -a newArr
k=0
for ((i=0;i<${#arr[@]};i++))
do
	if ((${arr[i]}!=-1))
	then
		count=1
		for ((j=i+1;j<${#arr[@]};j++))
		do
			if ((${arr[i]}==${arr[j]} && ${arr[j]}!=-1)) 
			then
				arr[j]=-1
				((count++))
			fi
		done
		element[k]=${arr[i]}
		newArr[k]=$count;
		((k++))
	fi
done
max=0
count1=0
echo ${mewArr[@]}
echo ${element[@]}
for ((i=0;i<${#newArr[@]};i++))
do
	if(( count1 < ${newArr[i]}))
	then
		max=${element[i]}
		count1=${newArr[i]}
	fi
done
echo "Maximum frecuency is " $max $count1
```

4. The code above first declare an array. Use nested Loop to find the frequency of each element and place -1 at visited element and store frequency and element in a new array. The find max by loop and display on shell.

5. change the permission to executable using `chmod uo+x Task1.sh`.

   > ######`Chmod Command`
   >
   > The command 	`chmod uo+x Lab4I.sh` changes the permissions of the file "Lab4I.sh" to make it executable. The `chmod` command is used to modify the permissions of a file or directory, and the `uo+x` option specifies that the user (owner) and others (all) should be given execute permission (+x) on the file. This means that the owner of the file and anyone else who has access to it can run the script by typing its name in the terminal. Without execute permission, the file cannot be executed and the user would see a "permission denied" error when trying to run it.

6. Run file using `bash Task1.sh`. The command runs the Bash script "Task1.sh" . 


   ![alt text for screen readers](images/Task1output.png)

#### Create a Bash script to find the largest element of a given array of integers.

1. Create a file named `touch Task2.sh.` 

   *This command creates a new empty file with the specified name. 

   ​				The syntax is **touch *newfilename****

2. Open file in nano using `nano Task2.sh`

   *This command opens the file in the nano text editor, which allows you to write and edit the Bash script.* Save and exit the file by pressing "Ctrl-X", then "Y", and then "Enter".

3. Write the code provided below:

```bash
#!/bin/bash

declare -a intArr
echo "Enter Total Numbers you want to enetr..."
read count
for ((i=0; i<count; i++)) do
	echo "Enter" $i"th number"
	read intArr[i]
	echo "Number entered is"  ${intArr[i]}
done
max=0
for ((i=0; i<count; i++)) do
	if ((max<intArr[i])) 
		then
		max=${intArr[i]}
	fi
done
echo "maximum is " $max
```

1. In the code above first loop input number of elements in array till Count entered by user in `read count`.

   > if [ condition ]
   > then
   >
   > **`code for true Condtion`**
   >
   > else
   >
   > **`code to execute if condition is false`**
   >
   > fi
   >
   > ```bash
   > for ((i=0; i<count; i++)) 
   > do
   > #Code
   > done
   > ```

2. change the permission to executable using `chmod uo+x Task3.sh`.

   > The command 	`chmod uo+x Lab4I.sh` changes the permissions of the file "Lab4I.sh" to make it executable. The `chmod` command is used to modify the permissions of a file or directory, and the `uo+x` option specifies that the user (owner) and others (all) should be given execute permission (+x) on the file. This means that the owner of the file and anyone else who has access to it can run the script by typing its name in the terminal. Without execute permission, the file cannot be executed and the user would see a "permission denied" error when trying to run it.
   >
   > You can use digits alternatively
   >
   > * The first digit represents the owner's permissions.
   > * The second digit represents the group's permissions.
   > * The third digit represents everyone else's permissions.
   >
   > Each digit can have a value from 0 to 7, which corresponds to a different set of permissions:
   >
   > | Digit | Permission | Description              |
   > | ----- | ---------- | ------------------------ |
   > | 0     | ---        | No permissions           |
   > | 1     | --x        | Execute only             |
   > | 2     | -w-        | Write only               |
   > | 3     | -wx        | Write and execute        |
   > | 4     | r--        | Read only                |
   > | 5     | r-x        | Read and execute         |
   > | 6     | rw-        | Read and write           |
   > | 7     | rwx        | Read, write, and execute |

3. Run file using `bash Task2.sh `or `.\Task2.sh`. The command runs the Bash script "Task2.sh" . 

   ​

   ![alt text for screen readers](images/Task2output.png)

####Create a Bash script to separate 0s and 1s from a given array of values 0 and 1.

1. Create a file named `touch Task3.sh.` 

   *This command creates a new empty file with the specified name. 

   ​				The syntax is **touch *newfilename****

2. Open file in nano using `nano Task3.sh`

   *This command opens the file in the nano text editor, which allows you to write and edit the Bash script.* Save and exit the file by pressing "Ctrl-X", then "Y", and then "Enter".

3. Write the code provided below:

```bash
#!/bin/bash

declare -a binArr
binArr=(1 0 0 1 0 0 1 0 1 0 1 0 1 0 1 0 1 1 0)
declare -a Arr
j=0
for ((i=0; i<${#binArr[@]}; i++)) do
	if ((${binArr[i]} == 0))
	 then
		Arr[j]=0
		((j++))
	fi
done
for ((i=0; i<${#binArr[@]}; i++)) do
	if ((${binArr[i]} == 1))
	 then
		Arr[j]=1
		((j++))
	fi
done
echo ${Arr[@]}
```

4. `declare -a` is use to declare an array . The first loop is used to separate zeros from `binarr` and move them into  the starting index of second array `Arr` and the 2nd loop move all the ones into the  second array.

> if [ condition ]
> then
>
> **`code for true Condtion`**
>
> else
>
> **`code to execute if condition is false`**
>
> ```bash
> for ((i=0; i<count; i++)) 
> do
> 		#Code
> done
> ```

4. change the permission to executable using `chmod uo+x Task3.sh`.

   > The command 	`chmod uo+x Lab4I.sh` changes the permissions of the file "Lab4I.sh" to make it executable. The `chmod` command is used to modify the permissions of a file or directory, and the `uo+x` option specifies that the user (owner) and others (all) should be given execute permission (+x) on the file. This means that the owner of the file and anyone else who has access to it can run the script by typing its name in the terminal. Without execute permission, the file cannot be executed and the user would see a "permission denied" error when trying to run it.
   >
   > You can use digits alternatively
   >
   > * The first digit represents the owner's permissions.
   > * The second digit represents the group's permissions.
   > * The third digit represents everyone else's permissions.
   >
   > Each digit can have a value from 0 to 7, which corresponds to a different set of permissions:
   >
   > | Digit | Permission | Description              |
   > | ----- | ---------- | ------------------------ |
   > | 0     | ---        | No permissions           |
   > | 1     | --x        | Execute only             |
   > | 2     | -w-        | Write only               |
   > | 3     | -wx        | Write and execute        |
   > | 4     | r--        | Read only                |
   > | 5     | r-x        | Read and execute         |
   > | 6     | rw-        | Read and write           |
   > | 7     | rwx        | Read, write, and execute |

5. Run file using `bash Task3.sh`. The command runs the Bash script "Task3.sh" . 

   ​

   ![alt text for screen readers](images/Task3output.png)

#### Create a Bash script to find the first repeating element in an array of integers.

1. Create a file named `touch Task4.sh.` 

   *This command creates a new empty file with the specified name. 

   ​				The syntax is **touch *newfilename****

2. Open file in nano using `nano Task4.sh`

   *This command opens the file in the nano text editor, which allows you to write and edit the Bash script.* Save and exit the file by pressing "Ctrl-X", then "Y", and then "Enter".

3. Write the code provided below:

```bash
#!/bin/bash

decalre -a arr
echo "How many elements you want to enetr..."
read count
for ((i=0;i<count ;i++))
do
	echo "Enter num " $((i+1))
	read arr[i]
done
for ((i=0; i<count; i++))
do
	for ((j=i+1; i<count; i++))
	do
		if ((${arr[i]}==${arr[j]}))
		then
			echo ${arr[i]} "is first  repeating element"
			exit
		fi
	done
done
```

4. `declare -a` is use to declare an array .The code above first ask user to enter desired numbers loop them to read from `shell` and then use nested loop to compare numbers. `exit` keyword is used to  exit from code. Alternatively you can use `break 2;`. which is used to break out of 2 loop inner and outer loop.

> if [ condition ]
> then
>
> **`code for true Condtion`**
>
> else
>
> **`code to execute if condition is false`**
>
> fi

>for var in list
>do
>  	**`Alternative for loop`** 
>done

5. change the permission to executable using `chmod uo+x Task4.sh`.

> ###### `Chmod Command`
>
> The command 	`chmod uo+x Lab4I.sh` changes the permissions of the file "Lab4I.sh" to make it executable. The `chmod` command is used to modify the permissions of a file or directory, and the `uo+x` option specifies that the user (owner) and others (all) should be given execute permission (+x) on the file. This means that the owner of the file and anyone else who has access to it can run the script by typing its name in the terminal. Without execute permission, the file cannot be executed and the user would see a "permission denied" error when trying to run it.
>
> You can use digits alternatively
>
> * The first digit represents the owner's permissions.
> * The second digit represents the group's permissions.
> * The third digit represents everyone else's permissions.
>
> Each digit can have a value from 0 to 7, which corresponds to a different set of permissions:
>
> | Digit | Permission | Description              |
> | ----- | ---------- | ------------------------ |
> | 0     | ---        | No permissions           |
> | 1     | --x        | Execute only             |
> | 2     | -w-        | Write only               |
> | 3     | -wx        | Write and execute        |
> | 4     | r--        | Read only                |
> | 5     | r-x        | Read and execute         |
> | 6     | rw-        | Read and write           |
> | 7     | rwx        | Read, write, and execute |

6. Run file using `bash Task4.sh` or `./Task4.sh`. The command runs the Bash script "Task4.sh" . 



![alt text for screen readers](images/Task4output.png)

