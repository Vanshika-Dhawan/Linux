A) Problem: Write Shell scripts to print system information

Step 1 - Open linux and create a new file using nano editor.

nano <file_name.sh>

![image](https://github.com/user-attachments/assets/3f255b0e-ae60-482c-807f-1c38a6e55ee0)

Step 2 - Now fill in the contents of the script and use the 'lscpu' command for diaplaying system information.

#!/bin/bash

echo $(lscpu)

Step 3 - Use bash command with script name to see the system info.

bash <file_name.sh>

![image](https://github.com/user-attachments/assets/0a83cb7b-fc9a-4a6a-9d92-d421f017d927)

B) Problem: Write Shell scripts to perform basic mathematical calculations.

Step 1 - Open linux and create a new file using nano editor.

nano <file_name.sh>

![image](https://github.com/user-attachments/assets/39bbbcc9-2e5e-4a55-b72b-c970f3ec7e88)


Step 2 - Update the contents of the file with the code below to create a calculator

#!/bin/bash

echo "Enter the first number: "
read a

echo "Enter the second number: "
read b

echo "Which operator do you want to use? (Enter the corresponding number)"
echo "1. '+' (Addition)"
echo "2. '-' (Subtraction)"
echo "3. '*' (Multiplication)"
echo "4. '/' (Division)"
read op

case $op in
  1)
    result=$((a + b))
    echo "Result: $a + $b = $result"
    ;;
  2)
    result=$((a - b))
    echo "Result: $a - $b = $result"
    ;;
  3)
    result=$((a * b))
    echo "Result: $a * $b = $result"
    ;;
  4)
    result=$((a / b))
    echo "Result: $a / $b = $result";;
  *)
    echo "Invalid";;
esac


![Screenshot 2025-03-25 110944](https://github.com/user-attachments/assets/3bbcc461-9def-44c0-9234-4f983c5b1c8b)


![Screenshot 2025-03-25 110953](https://github.com/user-attachments/assets/bcc98f6b-f55c-41c4-ae9d-3aabb7ffc224)


Step 3 - Now run the script using bash and start interacting.

bash <file_name.sh>

![image](https://github.com/user-attachments/assets/dfd0876b-41ff-43d5-9cc6-e535f8c1c497)

C) Problem: Use redirection command to store the output of commands.

Step 1 - Open linux and create a new file using touch command.

touch <filename.txt>

Step 2 - Now use the redirection operator to store the contents of the command in file & use the cat command to see the contents.

<command> > <file_name.sh>

![image](https://github.com/user-attachments/assets/e15d367f-668d-4c41-9a25-6e6785b9dc7d)






