# Lab Report 1

The following tutorial is designed for future CSE 15L students. It details how to log into a course-specific account on ieng6.

## Installing VScode

Firstly, you will need to go to the [Visual Studio Code website](https://code.visualstudio.com/).

![Image](vscodewebsite.png)

Make sure to download the appropriate version for your operating system. Upon the completion of the installation, you should be able to open VSCode
on your computer. Locate the menu at the top and hover your mouse over the Terminal tab, then click New Terminal.

![Image](vscodeopen.png)

## Remotely Connecting

Use the following [link](https://sdacs.ucsd.edu/~icc/index.php) to look up your course-specific account for CSE 15L.
Upon logging in with your TritonLink Username and PID, you should be presented with a page with the headline "Account Lookup Results."  Locate the section titled "Additional Accounts" and click on the button containing text beginning with `cse15lsp23.` Proceed to use the Global Password Change Tool(you will need your username beginning with `cse15lsp23` for this step). It may take several minutes for your password change to be completely processed.

After you've ensured that your password has successfully been reset, you will proceed to remotely connect to the server.

Note that if you're using Windows, you will need to install git for Windows using the following [link](https://gitforwindows.org/).

Run the following command in the terminal: `ssh <username>@ieng6.ucsd.edu`(replacing username with your specific username). Then enter your password.  If you are prompted with the question `Are you sure you want to continue connecting(yes/no/[fingerprint])?`, type yes.

![Image](remotelogin.png)

## Trying Some Commands

After connecting to the server, you can try running the following commands in the terminal:

* `cd ~`
<br>This command is intended to take you back to the home directory.
* `cd`
<br>This command is intended to change the current working directory.
* `ls -lat`
<br>This command is intended to display all files(both ones with permitted access and hidden ones), and sorts these files according to time.
* `ls -a`
<br>This command is intended to display hidden files.
* `ls <directory> where <directory> is /home/linux/ieng6/cs15lsp23/cs15lsp23abc, where the abc is one of the other group members’ username`
<br>This command is intended to list the files and folders in the directory of another group member's course-specific account for CSE 15L.
* `cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/`
<br>This command is intended to copy the file `hello.txt` into the specified home directory.
* `cat /home/linux/ieng6/cs15lsp23/public/hello.txt`
<br>This command is intended to read and output the contents of the file `hello.txt` contained in the cs15lsp23 folder.

![Image](commands.png)

This screenshot shows the results of running the specified commands above. The commands `cd ~` and `cd` took me back to my home directory. The command `ls -lat` printed out all files(hidden and unhidden) in the directory and sorted them according to time.  The command `ls -a` outputs the hidden files. The command `ls /home/linux/ieng6/cs15lsp23/cs15lsp23kav` failed as the directory doesn't exist. If the directory belonged to another individual's course-specific account for CSE 15L, the command wouldn't output the files and folders in that directory unless we have permission to access it. Lastly, the command `cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/` copied `hello.txt` into the specified directory, and `cat /home/linux/ieng6/cs15lsp23/public/hello.txt` outputted the contents of this file.

To log out of the remote server in your terminal, you can use:

* `Ctrl-D`
* `Run the command exit`
