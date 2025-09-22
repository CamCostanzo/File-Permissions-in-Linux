<img width="3840" height="2160" alt="image" src="https://github.com/user-attachments/assets/127ec07c-7bd0-4482-aca3-b3d91466e84c" />


# File-Permissions-in-Linux

## Check file and directory details
To check the permissions of the files and directories the ls -l command can be used to show the permissions for them. If there are hidden files we can show them using the ls -a command. To show all file permissions we can combine the two previous commands into ls -la. 
An example is shown below:


<img width="650" height="207" alt="port1" src="https://github.com/user-attachments/assets/d25988d6-ac39-44fa-8c38-a68b3fee75fe" />

## Describe the permissions string
Using the photo above and after performing the command to check the permissions we are given all the files and directories with their permissions. The 10-character string at the beginning of each entry is showing what type the entry is using; a ‘-’ represents a file and a ‘d’ represents a directory. The next 9 characters are split into different sections of people that can access the file or directory. The first is 2-4 and is the user, next 5-7 is the group, and 8-10 is the other.User is the person who created the file. Group can be a set of individuals working together. Other is any other person who can access the file. There are three permissions each section can have: r for read, w for write, and x for executable is applicable to the current entry.  For example the file project_k.txt is a file because it starts with a dash where the user has read and write permission, group has read and write permission, and other has read and write permission.

## Change file permissions
The file project_k.txt is giving the section other permissions to write, which is a security risk. We will need to change the permissions so they can no longer write. To do this we will use the chmod command. After writing chmod you will need to use either u,g, or o for user, group, and other followed by a ‘+’ or ‘-’ to give or take away permission. If you have to do more than one you separate each with a comma. Lastly put the file or directory you want these permission changes to be done on. 
An example is shown below:

<img width="705" height="392" alt="port2" src="https://github.com/user-attachments/assets/8ccb4bfb-7e80-4e9f-a33d-8f52d23b29cd" />


## Change file permissions on a hidden file
We need to change the permissions of the hidden file .project_x.txt . We know it's a hidden file because of the ‘.’ at the beginning of the name. As mentioned earlier you can only see this with the command ls -a or ls -la. The organization wants only the user and group to have only read permissions. A more efficient way to change a permission to only one access type is to use an ‘=’ after the section.
 Below will show how we complete this task:

 <img width="666" height="218" alt="port3" src="https://github.com/user-attachments/assets/fecafab7-f99f-4273-8e6e-ce2a03afbf82" />


## Change directory permissions
The directory drafts belong to the user researcher2 and they should be the only person with access to it. Looking at the permissions group also has permissions to this directory through executable. To change that we will use the chmod command again as shown below:

<img width="682" height="409" alt="port4" src="https://github.com/user-attachments/assets/65371ff3-24b6-4f2c-97ac-6ce9ac2f267a" />


## Summary
In this project we changed multiple permissions for files and directories in the projects directory. We accomplished this by using two commands the  ls -la  and chmod. Now that we have updated these permissions we have secured the system. 
