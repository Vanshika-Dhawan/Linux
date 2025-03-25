Problem: Implement ps, top, kill command with their options.Installing, updating, and removing software by apt-get command.

A) Process Management Commands

1. ps Command
   
The ps command is used to view information about processes running on the system.

Examples:

ps  

![image](https://github.com/user-attachments/assets/29f6703b-b8e8-4816-933c-66a73e6a0e0a)

ps -e 

![image](https://github.com/user-attachments/assets/8dc98040-dee6-46b9-ad56-b42f5de2ac27)

ps -f 

![image](https://github.com/user-attachments/assets/45ac37f2-8587-4099-a8de-59c7933753fa)


ps aux   


![image](https://github.com/user-attachments/assets/46b84bfc-0f91-45ec-b34a-1cacd942503e)


ps -ef | grep <process_name>  # Searches for a specific process

2. top Command
The top command provides a real-time view of system processes and their resource usage.

How to Use:

top                # Starts the top command

Key Options (Interactive Usage):

k: Kill a process by entering its PID.

h: Help menu for top.

u: Filter processes by a specific user.

q: Quit the top command.

![image](https://github.com/user-attachments/assets/937e23a9-c4d9-476e-969f-bdea7d45ce23)


3. kill Command
The kill command is used to terminate processes by their PID.

Examples:
ps -e               # Find the PID of a process
kill <PID>          # Kills the process with the given PID
kill -9 <PID>       # Force kills the process


Options:

-9: Sends the SIGKILL signal to forcefully terminate the process.

-15: Sends the SIGTERM signal to gracefully terminate the process.

B) Software Management Commands

1. Installing Software with apt-get
2. 
The apt-get command is used for managing software packages in Debian-based systems.

Installing a Package:

sudo apt-get update                  # Updates the list of available packages
sudo apt-get install <package_name>  # Installs the specified package


2. Updating Software with apt-get
3. 
sudo apt-get update       # Updates package information
sudo apt-get upgrade       # Installs newer versions of installed packages


4. Removing Software with apt-get
5. 
sudo apt-get remove <package_name>       # Removes the specified package
sudo apt-get purge <package_name>        # Removes the package and its configuration files



