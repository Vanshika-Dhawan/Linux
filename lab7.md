A) Implement chown, chmod command with their options.

Step 1 - Open Linux and create a new file using the touch command.

touch example_file.txt

![image](https://github.com/user-attachments/assets/492beb64-8652-4b2d-8249-9b30c80b5c12)

Step 2 - Change the ownership of the file.

chown username example_file.txt

Replace username with the desired user's name.

![image](https://github.com/user-attachments/assets/f555ff07-f53c-49a5-a63f-d356913cd4f7)

To change both owner and group, use:

chown username:groupname example_file.txt

Step 3 - Verify ownership change using ls -l.

ls -l example_file.txt

The output will show the updated owner and group of the file.

B) Problem: Change file permissions using chmod.

Step 1 - Create a file or directory.

touch another_file.txt

![image](https://github.com/user-attachments/assets/76a8a0e9-fd5c-4aa1-8c77-0707bda0a677)

Step 2 - Modify permissions using octal values.

chmod 755 another_file.txt

This sets the permissions as follows: -- Owner: Read, write, execute. -- Group: Read, execute. -- Others: Read, execute.

![image](https://github.com/user-attachments/assets/1f45e681-31dd-49aa-89c7-8a499a43f16d)

Step 3 - Verify the changes.

ls -l another_file.txt

The output will display the file permissions as -rwxr-xr-x.

![image](https://github.com/user-attachments/assets/0da3751f-082f-419b-9f54-af7ba4c8f937)






