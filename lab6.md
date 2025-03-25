Problem: Create the operator1 user and confirm that it exists in the system. Set the password for operator1. Create the additional operator2 and operator3 users. Set their passwords aswell. Run the usermod -c command to update the components of the operator1 user account. Remove the operator3 user from the system.

Step 1 - Create a new user

sudo useradd operator1

Step 2 - Setting the password for operator1

sudo passwd operator1

![image](https://github.com/user-attachments/assets/c550999f-aed1-4001-be59-d7a3a626ebb5)


Step 3 - Create two more users operator2 & operator3
sudo useradd operator2
sudo useradd operator3

![image](https://github.com/user-attachments/assets/02aee1ea-8115-4ca6-89bc-bab2fa385474)

Step 4 - Setting the passwords for operator2 & operator3

sudo useradd operator2
sudo useradd operator3

Step 5 - Set the comments of the user operator 

sudo usermod -c "Doing lab 12" operator1
getent passwd operator1

![image](https://github.com/user-attachments/assets/4b7d4d7b-8e43-4185-9bb7-6ef7b81ccc82)

Step 6 - Remove operator 3 and view the updated users list

sudo userdel operator3
getent passwd

![image](https://github.com/user-attachments/assets/e831847f-55f4-4d30-8660-167d230a31c8)


