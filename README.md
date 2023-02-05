# command_line_assignment
This is the command line assignment

### Question - 1
Write a bash script to get the current date, time, username, home directory and current working directory.

#### Apporach - 
We have used the following commands to fetch the desired details, each command is as below.
| Command  | Function |
| ------------- | ------------- |
|$(date +"Year: %Y, Month: %m, Day: %d") | Command to fetch the date
|$(date +"%T") | Command to fetch the time
|$(whoami) | Command to fetch the current working user
|$(echo $HOME) | Command to fetch the Home directory
|$(pwd) | Command to fetch the current wokring directory


###Output ScreenShot-


<img width="493" alt="Screenshot 2023-02-05 at 2 53 27 PM" src="https://user-images.githubusercontent.com/122472996/216811264-7ddbc37c-bcc3-48cf-bcfc-d4da452f8a1a.png">


### Question - 2
Write a bash script (name Table.sh) to print the Table of a number by using a while loop. It should support the following requirements.
  - The script should accept the input from the command line.
  - If you don’t input any data, then display an error message to execute the script correctly.

#### Apporach - 

We verify whether any arguments have been passed, and if not, we issue an error and quit the programme with exit status 1. If not, we run a loop to print all the arguments passed, then another while loop on all the arguments, start a counter internally on the second while loop, increment it after each iteration, fetch the result, and repeat this internal loop for each element in the arguments list until the counter value is less than 10, at which point the programme ends.


###Output ScreenShot-

<img width="548" alt="Screenshot 2023-02-05 at 3 02 03 PM" src="https://user-images.githubusercontent.com/122472996/216811613-708a43dc-0351-4aa5-9ec8-bde29001d357.png">

### Question - 3
Write a Function in bash script to check if the number is prime or not? It should support the following requirement.
          - The script should accept the input from the User.
#### Apporach - 

We created a function called `is prime` to determine whether a number is prime or not. If the number is less than 2, we indicate that it is not a prime, and if not, we run a loop from `2` to `number/2+1` to see if any of the above numbers divide the given number. If we found any numbers, we can conclude that the number is not a prime because it has a divisor other than 1 and itself.

We receive user input in the main code, store it in a variable, and then call the function while sending the argument as command line arguments.

###Output Screenshot-

<img width="401" alt="Screenshot 2023-02-05 at 3 08 16 PM" src="https://user-images.githubusercontent.com/122472996/216811823-c41fab8d-22bd-4439-9ef7-7d8784ce3c04.png">

### Question - 4
Create a bash script that supports the following requirement.
  - Create a folder ‘Assignment’.
  - Create a file ‘File1.txt’ inside ‘Assignment’ Folder.
  - Copy all the content of Table.sh(2nd script) in ‘File1.txt’ without using ‘cp’ and ‘mv’ command.
  - Append the text Welcome to Sigmoid’ to the ‘File1.txt’ file.
  - List all the directories and files present inside Desktop Folder.#### Apporach - 

#### Approach - 

We have used the following commands to meet the desired requirements and the function of command is as follows.
| Command  | Function |
| ------------- | ------------- |
| mkdir ~/Desktop/Assignment | Creating folder using mkdir |
| touch ~/Desktop/Assignment/File1.txt | Creating file using touch |
| cat ~/Desktop/Table.sh  >> ~/Desktop/Assignment/File1.txt | Copying data in q2 to file1 using cat |
| echo "Welcome to Sigmoid" >> ~/Desktop/Assignment/File1.txt| Appending given text to file1 |
| ls -la ~/Desktop/ | Printing files and folders in Desktop |


<img width="660" alt="Screenshot 2023-02-05 at 3 12 17 PM" src="https://user-images.githubusercontent.com/122472996/216811923-64a27e0d-cb2d-4c12-a936-d5061f140d24.png">

### Question - 5
You have given an array. Using Bash script, print its length, maximum element and
minimum element.
		arr=( 2 3 4 1 6 7).
#### Approach - 

We have declared the array internally in the code, we have used the following commands to fetch the required result

####Output ScreenShot -
<img width="630" alt="Screenshot 2023-02-05 at 3 16 52 PM" src="https://user-images.githubusercontent.com/122472996/216812093-05d4c50e-1727-48d1-919d-7e9a17aeb67f.png">



