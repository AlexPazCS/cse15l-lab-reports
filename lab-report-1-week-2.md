# How to use SSH / remote connect
## Download and install VS Code </brk>
Go [here](https://code.visualstudio.com/download) to download and install VS Code.
![Image](https://user-images.githubusercontent.com/103294574/162673092-83a6d8b2-a7d4-475f-9152-6eedd1069b29.png)
## Use shh and input your username, server, and password
Input `$ ssh` followed up by your username, in my case its `cs15lsp22ald` then `@` and finally the server which is `ieng6.ucsd.edu`. The result should look like this: `ssh cs15lsp22ald@ieng6.ucsd.edu`. </brk>
![Link](https://user-images.githubusercontent.com/103294574/162673237-c148ceeb-ddd3-4b2d-96f6-44318269a459.png)
## Try out ssh commands in terminal 
You can use these handy commands:
- `cd` to go to a directory
- `ls` to view the contents of the directory
- `touch` to make a file in the current directory
- `mkdir` to make a new directory in the current directory
- `rm` to remove a file 
- `cp` to copy a file 
- `mv` to move a file 

![image](https://user-images.githubusercontent.com/103294574/162676015-7d4341b4-b9b8-4eee-b540-f16591e9e97a.png)
# Moving files from personal device to server using scp command
type `scp` followed by the file you want moved, so in my case `Main.java` followed by your username and server address like you did before, with the directory you want the file to be in inputted as `: <directory>`
![image](https://user-images.githubusercontent.com/103294574/162678179-b8dd42b6-29d2-4f8e-81d8-a99e3efe5f60.png)
# Making a keygen to save time
type in `ssh-keygen` in the terminal and chosoe the file location in the parenthesis. Then put in your password and now you have a keygen on your local pc. To move this using ssh, you must make a .ssh file in the root of your connected server and go back to client. type `scp` the file location your keygen is, then your username and server and `:~/.ssh/authorized_keys`
![image](https://user-images.githubusercontent.com/103294574/162681580-a291d230-2139-4706-b4fb-63e536eca25a.png)
