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
<img src="https://imgur.com/a/0wpo4pp" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

The first two lines of the screenshot display the commands I entered, and the other lines display the output of the second command. 
The chmod command changes the permissions on files and directories. The first argument indicates what permissions should be changed, and the second argument specifies the file or directory. 
In this example, I removed write permissions from other for the project_k.txt file. After this, I used ls -la to review the updates I made.
