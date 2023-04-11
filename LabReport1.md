**Lab Report 1**
---
How to log into a course-specific account on ieng6?
---
1. Downloading VScode
- Open [VScode website](https://code.visualstudio.com/). 
- Download suitable package ( windows/ macos).
- Follow the instructions to complete setup.
Below is how your screen must look like after you complete setup.
<img width="1440" alt="VScodeOpenPage" src="https://user-images.githubusercontent.com/130006438/231030770-1fe47eef-af77-4154-b264-7f8f06767251.png">

2. Remotely Connecting

- Go to terminal.
- Open a new terminal.
- It must look like this:

<img width="1440" alt="image" src="https://user-images.githubusercontent.com/130006438/231030993-c31a163e-e54f-4d06-982f-0cf8023b4fc1.png">

- Next, type this in the terminal and replace ***zz*** with the letters in your course-specific account 

>  ssh cs15lsp23zz@ieng6.ucsd.edu

Type yes when you see this:
```
The authenticity of host "ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHHAtLUHngrPEZTD1/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```

Log in is now complete.
Your screen must look like this:

<img width="740" alt="Screenshot 2023-04-10 at 7 24 01 PM" src="https://user-images.githubusercontent.com/130006438/231039295-9d3ad65c-5453-4468-9452-8ad6b64e0bf5.png">

 Trying Some Commands

- cd~
- cd
- ls -lat
- ls -a
- ls <directory>
- cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/
- cat /home/linux/ieng6/cs15lsp23/public/hello.txt

 ---
Some examples:
  
<img width="740" alt="Screenshot 2023-04-10 at 9 42 11 PM" src="https://user-images.githubusercontent.com/130006438/231058221-3c9a28a9-0c06-47a7-bce3-27c2cb44eb08.png">
 
