# Lab Report 4

## Step 4
![Image](Step4.png)
<br><br>To get to this step, I started a new terminal and typed in the command `ssh cs15lsp23ks@ieng6.ucsd.edu` to login to my CSE 15L account. I pressed `<enter>` to run the command.

## Step 5
![Image](Step5.png)
<br><br>To get to this step, I typed the command `git clone https://github.com/ucsd-cse15l-s23/lab7` in the terminal. I pressed `<enter>` to run the command.

## Step 6
![Image](Step6.png)
<br><br>To demonstrate that the tests contained in `ListExamples.java` fail, I typed the command `bash test.sh` in the terminal. I pressed `<enter>` to run the command.

## Step 7
![Image](Step7-1.png)
<br><br>To edit the code file `ListExamples.java` to fix the error, I first ran the command `cd lab7` to change the working directory to `lab7`. I then typed in `vim ListExamples.java` to directly edit the file.

![Image](Step7-2.png)
<br><br>I was presented with the code above after running the command `vim ListExamples.java`. The screenshot and details below show the keys that I pressed to fix the error.

![Image](Step7-3.png)
<br><br>I first pressed the up arrow/`k` to reach the line containing the error.  I then pressed the right arrow/`l` until my cursor was over the `1` in `index1`, and I pressed `x` to delete the `1`. I proceeded to press `i` to enter the insert mode, and pressed `2` so that the line now contains `index2`. I pressed `<esc>` to exit the insert mode, and then I pressed `:wq` followed by `<enter>` to save my changes.

## Step 8
![Image](Step8.png)
<br><br>I returned to the terminal and I ran the command `bash test.sh` to demonstrate that the error has been fixed and the tests now succeed.

## Step 9
![Image](Step9-1.png)
<br><br>I ran the command `git add ListExamples.java` to stage the file in order to commit it to GitHub. To confirm that my changes have been appropriately saved, I ran the command `git status`. I then ran the command `git push https://github.com/emilynpark/lab7` to push the changes to my GitHub account.

![Image](Step9-2.png)
<br><br>The resulting changes have been successfully saved to my GitHub account.
