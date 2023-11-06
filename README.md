<h1># Linux Permissions Project </h1>

<h2>Description</h2>
The research team at my organisation needs to update the file permissions for certain files and directories within the projects directory. The permissions do not currently reflect the level of authorisation that should be given. Checking and updating these permissions will help keep their system secure. To complete this task, I performed the following tasks:
<br />


<h2>Languages and Utilities Used</h2>

- <b>BashShell</b> 
  

<h2>Environments Used </h2>

- <b>Linux</b>
  

<h2>Check file and directory details:</h2> <br/>

The organisation determined that other shouldn't have write access to any of their files. To comply with this, I referred to the file permissions that I previously returned. I determined project_k.txt must have the write access removed for other.

The following code demonstrates how I used Linux commands to do this:

<p align="center">
<img src="https://imgur.com/ARiJAR0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

The first two lines of the screenshot display the commands I entered, and the other lines display the output of the second command. 
The chmod command changes the permissions on files and directories. The first argument indicates what permissions should be changed, and the second argument specifies the file or directory. 
In this example, I removed write permissions from other for the project_k.txt file. After this, I used ls -la to review the updates I made.

<h2>Describe the permissions string:</h2> <br/>

The 10-character string can be deconstructed to determine who is authorised to access the file and their specific permissions. The characters and what they represent are as follows:

●	1st character: This character is either a d or hyphen (-) and indicates the file type. If it’s a d, it’s a directory. If it’s a hyphen (-), it’s a regular file.

●	2nd-4th characters: These characters indicate the read (r), write (w), and execute (x) permissions for the user. When one of these characters is a hyphen (-) instead, it indicates that this permission is not granted to the user.

●	5th-7th characters: These characters indicate the read (r), write (w), and execute (x) permissions for the group. When one of these characters is a hyphen (-) instead, it indicates that this permission is not granted for the group.

●	8th-10th characters: These characters indicate the read (r), write (w), and execute (x) permissions for other. This owner type consists of all other users on the system apart from the user and the group. When one of these characters is a hyphen (-) instead, that indicates that this permission is not granted for other.

For example, the file permissions for project_t.txt are -rw-rw-r--. Since the first character is a hyphen (-), this indicates that project_t.txt is a file, not a directory. The second, fifth, and eighth characters are all r, which indicates that user, group, and other all have read permissions. The third and sixth characters are w, which indicates that only the user and group have write permissions. No one has execute permissions for project_t.txt.

<h2>Change file permissions:</h2> <br/>

The organisation determined that other shouldn't have write access to any of their files. To comply with this, I referred to the file permissions that I previously returned. I determined project_k.txt must have the write access removed for other.

The following code demonstrates how I used Linux commands to do this:

<p align="center">
<img src="https://imgur.com/7bFJqnk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

The first two lines of the screenshot display the commands I entered, and the other lines display the output of the second command. The chmod command changes the permissions on files and directories. The first argument indicates what permissions should be changed, and the second argument specifies the file or directory. In this example, I removed write permissions from other for the project_k.txt file. After this, I used ls -la to review the updates I made.
