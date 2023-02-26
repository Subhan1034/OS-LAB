

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

declare -a intArr
echo "Enter Total Numbers you want to enetr..."
read count
for ((i=0; i<count; i++)) do
	echo "Enter" $i "th number"
	read intArr[i]
	echo "Number entered is"  ${intArr[i]}
done
maxCount=0
maxElement=""
for i in "${!intArr[@]}"; do
  if (( ${intArr[$i]} > $maxCount ))
  then
    maxCount=${count[$i]}
    maxElement=$i
  fi
done
echo "maximum is " $maxElement
```

4. The code above first use **\$1,\$2 and \$3** as  command line arguments. The compare them using if in bash script and then print largest of them.

   >if [ condition ]
   >then
   >
   >**`code for true Condtion`**
   >
   >else
   >
   >**`code to execute if condition is false`**
   >
   >fi

5. change the permission to executable using `chmod uo+x Task1.sh`.

   > ######`Chmod Command`
   >
   > The command 	`chmod uo+x Lab4I.sh` changes the permissions of the file "Lab4I.sh" to make it executable. The `chmod` command is used to modify the permissions of a file or directory, and the `uo+x` option specifies that the user (owner) and others (all) should be given execute permission (+x) on the file. This means that the owner of the file and anyone else who has access to it can run the script by typing its name in the terminal. Without execute permission, the file cannot be executed and the user would see a "permission denied" error when trying to run it.

6. Run file using `bash Task4.sh`. The command runs the Bash script "Task4.sh" . 

    ​

   ![alt text for screen readers](..\Task1output.png)

#### Create a Bash script to find the largest element of a given array of integers.

1. Create a file named `touch Task1.sh.` 

   *This command creates a new empty file with the specified name. 

   ​				The syntax is **touch *newfilename****

2. Open file in nano using `nano Task1.sh`

   *This command opens the file in the nano text editor, which allows you to write and edit the Bash script.* Save and exit the file by pressing "Ctrl-X", then "Y", and then "Enter".

3. Write the code provided below:

```
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

2. change the permission to executable using `chmod uo+x Task1.sh`.

   > ###### `Chmod Command`
   >
   > The command 	`chmod uo+x Lab4I.sh` changes the permissions of the file "Lab4I.sh" to make it executable. The `chmod` command is used to modify the permissions of a file or directory, and the `uo+x` option specifies that the user (owner) and others (all) should be given execute permission (+x) on the file. This means that the owner of the file and anyone else who has access to it can run the script by typing its name in the terminal. Without execute permission, the file cannot be executed and the user would see a "permission denied" error when trying to run it.

3. Run file using `bash Task4.sh`. The command runs the Bash script "Task4.sh" . 

   ​

   ![alt text for screen readers](images/Task2output.png)

####Create a Bash script to separate 0s and 1s from a given array of values 0 and 1.

1. Create a file named `touch Task1.sh.` 

   *This command creates a new empty file with the specified name. 

   ​				The syntax is **touch *newfilename****

2. Open file in nano using `nano Task1.sh`

   *This command opens the file in the nano text editor, which allows you to write and edit the Bash script.* Save and exit the file by pressing "Ctrl-X", then "Y", and then "Enter".

3. Write the code provided below:

```
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

1. change the permission to executable using `chmod uo+x Task1.sh`.

   > ###### `Chmod Command`
   >
   > The command 	`chmod uo+x Lab4I.sh` changes the permissions of the file "Lab4I.sh" to make it executable. The `chmod` command is used to modify the permissions of a file or directory, and the `uo+x` option specifies that the user (owner) and others (all) should be given execute permission (+x) on the file. This means that the owner of the file and anyone else who has access to it can run the script by typing its name in the terminal. Without execute permission, the file cannot be executed and the user would see a "permission denied" error when trying to run it.

2. Run file using `bash Task4.sh`. The command runs the Bash script "Task4.sh" . 

   ​

   ![alt text for screen readers](images/Task3output.png)

#### Create a Bash script to find the first repeating element in an array of integers.

1. Create a file named `touch Task1.sh.` 

   *This command creates a new empty file with the specified name. 

   ​				The syntax is **touch *newfilename****

2. Open file in nano using `nano Task1.sh`

   *This command opens the file in the nano text editor, which allows you to write and edit the Bash script.* Save and exit the file by pressing "Ctrl-X", then "Y", and then "Enter".

3. Write the code provided below:

```
declare -a intArr
echo "Enter Total Numbers you want to enetr..."
read count
for ((i=0; i<count; i++)) do
	echo "Enter" $i "th number"
	read intArr[i]
	echo "Number entered is"  ${intArr[i]}
done
for i in "${intArr[@]}"; do
    (( counts[$i]++ ))
done

for i in "${intArr[@]}"; do
    if (( counts[$i] > 1 )); then
        echo "Element $i"
        break
    fi
done
```

1. The code above first use **\$1,\$2 and \$3** as  command line arguments. The compare them using if in bash script and then print largest of them.

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

2. change the permission to executable using `chmod uo+x Task1.sh`.

   > ###### `Chmod Command`
   >
   > The command 	`chmod uo+x Lab4I.sh` changes the permissions of the file "Lab4I.sh" to make it executable. The `chmod` command is used to modify the permissions of a file or directory, and the `uo+x` option specifies that the user (owner) and others (all) should be given execute permission (+x) on the file. This means that the owner of the file and anyone else who has access to it can run the script by typing its name in the terminal. Without execute permission, the file cannot be executed and the user would see a "permission denied" error when trying to run it.

3. Run file using `bash Task4.sh`. The command runs the Bash script "Task4.sh" . 

   ​

   ![alt text for screen readers](images/Task1output.png)

