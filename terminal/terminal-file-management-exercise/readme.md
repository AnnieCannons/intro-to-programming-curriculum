# Terminal File Management Exercise

An exercise on using a terminal to manage files.

## Learning Objectives

After this exercise, students should be able to:

- Launch the terminal program on their machine.
- See the contents of a folder with `ls` and compare those contents to what they see in the file manager
- Check where they are using `pwd` or the information in their prompt.
- Have some idea on how to look up more complex commands.

## Introduction

Today you're going to get some **practice** with using the terminal, but you are _not_ expected to memorize commands.

Instead, you should get some **exposure** to those commands, so that they will _begin_ to be familiar to you.

You will also gain some degree of familiarity with the command prompt—the place where you enter commands in a terminal. How it works, what its limitations are, and how to work within them.

Make sure you're being patient with yourself!

## How To Get Unstuck When Attempting These Tasks

You **may or may not** remember how to create a directory. If you're stuck, the answer is _not in your heart_. Ask a **friendly internet search engine** and read **several** posts to make sure you're getting **good and usable information**, or ask **another student**. If you're truly stuck, ask your **#help** channel in Slack. If you have to look it up often, that's okay! If you look it up often enough, you'll memorize the fact that the command is `mkdir`. If you don't memorize it, you probably aren't using it enough to need to!

**None of this asking other people is cheating.** You're practicing how to get yourself unstuck, how to research, and how to use the resources you have around you.

## Tasks


1. Think about the question, "What is the terminal?" Review the slide deck on the Terminal until you find an answer on this.
2. Where is your terminal located? Google ‘open terminal mac’ and make sure you know how to launch it!
3. Launch your terminal. If you've already got it open, switch to it and run the command `cd ~`, which navigates you to your "home directory". Use `pwd` to get your current working directory. It should print your home directory—`pwd` should give you a an output  of `/Users/` followed by your username on your computer. **Keep in mind that the home directory can also be shortened to "~"**, which is how we could say `cd ~`, which means "change directory to home". When you see the `~`, or `/Users/` followed by your username, remember that that's "home".
4. Use a terminal command to create a new directory called `my-files`.  Your current working directory won't change—run `pwd` to see that you're estill in your home directory. You can confirm that it worked by running `ls` to see the directory among the list of files and directories within your home directory.
5. Use a terminal command to navigate into the `my-files` directory. If you run `pwd`, you should now see a working directory file path that ends with `/my-files`. Use `ls` to see that the directory is empty—you should get no output.
6. Use a terminal command to create a new file called `file-1.txt`. If you run `ls` now, you should see `file-1.txt` as the only output.
7. Use a terminal command to create a new file called `file-2.txt`. If you run `ls` now, you should see `file-1.txt` and `file-2.txt` outputted.
8. Use a terminal command to create a new directory called `my-images`. Running `pwd` will still give you the same directory, since you haven't changed directories. But if you run `ls`, you should now see `file-1.txt`, `file-2.txt`, and `my-images` outputted.
9. Use a terminal command to create a new directory called `my-gifs`. Running `pwd` will still give you the same directory, since you haven't changed directories. But if you run `ls`, you should now see `file-1.txt`, `file-2.txt`, `my-images`, and `my-gifs` outputted.
10. Use a terminal command to navigate into the `my-images` directory. You should now be inside the `my-images` directory—confirm with `pwd`.
11. Create a new file called `image-1.png`. Your file system should now have a new file called `image-1.png` inside the `my-images` directory—confirm with `ls`.
12. Navigate back to the parent directory (`my-files`). You can do this by navigating back to your home directory and then into `my-files`, but there's a shortcut to navigating to your parent directory if you remember... or you can look it up! Either way, you should now be back inside the `my-files` directory—confirm this with `pwd`.
13. Run `history -n 20`. This will print out the last 20 commands you entered in your terminal. Could you have achieved the same results with fewer commands? If you want to restart to get a better "score", navigate back to your home directory and run `rm -rf my-files` to delete the directory and start back at the first step. **Any research you do** here will help you in your terminal journey—as well as help you **become a better researcher**!
14. Finally, copy and paste the text output from your terminal from `history -n 20` as your submission for this assignment. Well done!

## Extra Practice

You do **not** have to do the following tasks. They are **not an assignment** and **will not** be graded.

15. Use a terminal command to move the `my-gifs` directory into the `my-images` directory. Your file system should now have a directory called `my-gifs` _inside_ the `my-images` directory. You can confirm this by running `ls my-images`—this will keep you in your current directory while checking the contents of the `my-images` directory.
16. Use a terminal command to navigate into the `my-gifs` directory, keeping in mind that it's _within_ the `my-images` directory.
17. Use a terminal command to create a new file called `homer.gif`. Run `ls` to confirm it exists.
18. Use a terminal command to navigate back to your home directory and run an `ls` to confirm that the `my-files` directory is there. Use a terminal command to rename the `my-files` directory to `our-files`. You may have to do some research as to how to rename a file... but it actually uses a command you've already used. Run an `ls` command to confirm that your directory has an `our-files` directory and no `my-files` directory.
19. Use terminal commands to navigate into `our-files` and create new files called `file-3.txt` and  `file-4.txt`. Run `ls` to see if they were created and to see what else is in your current directory. Did you expect to see those results? Why or why not?
20. Use a terminal command to create a new directory called `my-scripts`. Run an `ls` to confirm it's been added.
21. Use a terminal command to navigate into the `my-scripts` directory. Run `pwd` to confirm.
22. Run the following command in your terminal. Watch the quotes and apostrophes!

```
echo 'echo "This is my first shell script!"' > script-1.sh
```

`echo` can insert text into a file, creating it if necessary. Run an `ls` and you should see that the file exists. Open the file in a text editor to see what text you've inserted.

23. Run the following command: 

```
chmod +x script-1.sh
```

This gives the script the ability to run as a program.

24. Run the following command: 

```
./script-1.sh
```

This will execute your program. You will see "This is my first shell script!" printed in your terminal.

25. Run `history -n 40`. This will print out the last 40 commands you entered in your terminal. Could you have achieved the same results with fewer commands? If you want to restart to get a better "score", navigate back to your home directory and run `rm -rf our-files` to delete the directory and start back at the first step. One thing to try is to run `ls`with a directory name as an argument to check contents of a directory _without_ having to enter a separate command to navigate into that directory. Feel free to research how you could navigate into a directory inside another directory in one command. **Any research you do** here will help you in your terminal journey—as well as help you **become a better researcher**!
26. Finally and **optionally**, copy and paste the output from `history -n 40` and DM it to your instructor for a 👍.
