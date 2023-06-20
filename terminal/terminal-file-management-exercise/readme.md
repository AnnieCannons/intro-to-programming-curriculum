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

## Tasks

1. Create a new directory called `my-files`. Your file system should now have a new directory called `my-files`
2. Navigate to the `my-files` directory. You should now be inside the `my-files` directory.
3. Create a new file called `file-1.txt`. Your file system should now have a new file called `file-1.txt` inside the `my-files` directory.
4. Create a new file called `file-2.txt`. Your file system should now have a new file called `file-2.txt` inside the `my-files` directory.
5. Create a new directory called `my-images`. Your file system should now have a new directory called `my-images` inside the `my-files` directory.
6. Navigate to the `my-images` directory. You should now be inside the `my-images` directory.
7. Create a new file called `image-1.png`. Your file system should now have a new file called `image-1.png` inside the `my-images` directory.
8. Navigate back to the parent directory. You should now be back inside the `my-files` directory.
9. Move the `my-images` directory into the `my-files` directory. Your file system should now have a new directory called `my-images` inside the `my-files` directory and no longer exist as a separate entity.
10. Rename the `my-files` directory to `our-files`. Your file system should now have a new directory called `our-files`.
11. Create a new file called `file-3.txt`. Your file system should now have a new file called `file-3.txt` inside the `our-files` directory.
12. Create a new file called `file-4.txt`. Your file system should now have a new file called `file-4.txt` inside the `our-files` directory.
13. Navigate to the `our-files` directory. You should now be inside the `our-files` directory.
14. Create a new directory called `my-scripts`. Your file system should now have a new directory called `my-scripts` inside the `our-files` directory.
15. Navigate to the `my-scripts` directory. You should now be inside the `my-scripts` directory.
16. Run the following command: 

```
echo 'echo "Hello World!"' > script-1.sh
```

Your file system should now have a new script file called script-1.sh with "echo "Hello World!"" written in it, located in your my-scripts folder.

17. Navigate back to the parent directory. You should now be back inside the our-files folder.
18. Move the our-files folder into your home folder. Your home folder should now contain a folder named our-files with all of its contents.
19. Navigate to your home folder. You should now be in your home folder.
20. Run the following command:

```
echo 'echo "This is my first shell script!"' > script-1.sh
```

Your home folder should now contain a script named script-1.sh with "echo "This is my first shell script!"" written in it.

21. Open your terminal and navigate to your home folder.
22. Run the following command: 

```
chmod +x script-1.sh
```

23. Run the following command: 

```
./script-1.sh
```

You will see "This is my first shell script!" printed in your terminal.
