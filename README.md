# shell script example for case statement 

## it prints the output that we chose 
#### first create a file 
#### then paste the script
#### you can even edit the script as you want 
```
#!/bin/bash

echo 
echo please chose one of the options below
echo
echo 'a = Display date and time'
echo
echo 'b = List files and directories'
echo 
echo 'c = list user logged in'
echo 
echo 'd = check system uptime'
echo 

	read choices
  	case $choices in 
a) date;;
b) ls -l ;;
c) cat /etc/passwd | more;;
d) uptime;;
*) echo invalid choice
        	esac	 
```
### for shell script 
```
#!/bin/bash
``` 
##### this should be at first of the file it staes it's a shell script 
##### echo is used to print the following words that we want to print in single or doubble quotations for example
```
echo 'this is an example'
```
##### the echo is used to make space between the line
```
echo
```
##### 
##### after editing save the file and change the permissions using chmod 
```
chmod a+x filename
```
##### then exicute the file 
##### to execute the file use this command
```
./filename
```
##### states the present directory 
##### to execute the script from other directory the give the full path of that file 
