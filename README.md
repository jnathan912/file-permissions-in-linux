# Managing File Permissions and Compliance in a Linux Environment


## Project description

In this project, I will check the permissions set for files and subdirectories in the “projects” directory. I'll make sure that I display all permissions, including hidden files. 
There are three permissions in Linux: Read (contents on the file can be read), write (allows modifications of contents of the file), and execute (enter a directory and access its files).

Each line will describe the permission granted for a file or directory for an owner. An owner can be a user, a group, or all other users on a system. 
  

## Check file and directory details

![image](https://github.com/user-attachments/assets/4721d6e2-f15e-401c-acc0-bebffb6e60c8)



## Description of the permissions string

A 10-character string represents file and directory permissions. The first letter is the file type. D is for directory and a hyphen (-) is for a regular file. The second, third, and fourth letters indicate the permissions for the user. The fifth, sixth, and seventh letters indicate the permissions for a group and the eighth, ninth, and tenth letters indicate the permissions for all others. 

R is for read, w is for write, and x is for execute. A hyphen would replace a letter if someone doesn’t have permission. 

Example 1. The first line indicates that the user has authorization to read, write, and execute the directory. The group and all others can read and execute the directory, but not write.

Example 2. The third line indicates that the user has read and write permissions for a file. A group has permission to write, and all others have no permission at all for the file. 


## Change file permissions

The organization does not allow all others to have write access to any files. I'll have to identify and update the file that needs to have its permissions modified.

![image](https://github.com/user-attachments/assets/14231734-cfd6-4a56-88c1-f14f19db47e8)



## Change file permissions on a hidden file

The research team has archived .project_x.txt, which is why it’s a hidden file. I've been advised that this file should not have write permissions for anyone, but the user and group should be able to read the file. 

![image](https://github.com/user-attachments/assets/3a076a4f-5d1f-49c0-9e24-3e965d546b0a)



## Change directory permissions

The files and directories in the projects directory belong to the researcher2 user. I'll make sure that only researcher2 will be allowed to access the drafts directory and its contents. 

![image](https://github.com/user-attachments/assets/0923b725-bfcb-4994-a9c5-e4112ddd3b2e)



## Summary

First, I checked and displayed the permissions for files and subdirectories in the projects directory, ensuring I included hidden files. Following that, I described the 10-character permission string for two examples from the output. Next, I identified a file that didn't comply with our organization's policy of not allowing 'other' users to have write access and then modified its permission. Additionally, I made sure that the hidden file '.project_x.txt' in our research team's possession only had read permissions for users and groups. Lastly, I modified the permissions in the 'drafts' directory to restrict access only to the 'researcher2' user.
