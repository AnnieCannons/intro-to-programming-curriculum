# Terminal Paths In-Class Group Exercise

An exercise on using a terminal to manage files.

## Learning Objectives

After this exercise, students should be able to:

- Identify a relative path and an absolute path.

## Introduction

Welcome to our file management exercise! In this exercise, we'll be exploring different kinds of file paths using our terminal. Before we get started, let's go over some basic concepts.

Understanding the difference between relative paths and absolute paths can help you greatly in:

- visualizing the file system
- figuring out why a file path didn't work
- writing complex file paths with speed and confidence (eventually!)

There are two types of file paths: **relative** paths and **absolute** paths. A relative path is a path that is relative **to the current working directory**. An absolute path is a path that **starts from the root directory**.

A **relative path** does not _have_ to start with a `./`, but it's a good reminder that we're still dealing with a path.

An **absolute path** _does_ have to start with a `/`. Sometimes you may start one with `~`, but that is a shortcut for `/Users/[username]`, which, as you can see, still starts with a `/`.

Here are some examples of relative and absolute paths:

### Relative Paths

- `./my_file.txt`
- `../Documents`
- `./Downloads/index.html`
- `../../Documents/dev/style.css`

### Absolute Paths

- `/Users/abbreviatedman/my_file.txt`
- `~/Documents/dev/style.css`
- `/Applications/Chrome`

In this exercise, we'll be using different kinds of file paths to manage files and directories. We'll be using relative paths, absolute paths, `~`, and `..`. When starting a relative path, all our examples should begin with `./` to remind us that we're using a relative path.

## How Do I Know I'm Doing It Right?

The two most important commands to memorize are `ls` and `pwd`—and if you have certain Oh-My-Zsh themes installed, they'll show you the output of `pwd` automatically, and then you only need `ls`.

Use `ls` to know **what contents your current directory has**, and `pwd` to know **the absolute path to your current directory**.

## Steps

Here are the steps you should follow during this exercise:

1. Open your terminal and navigate to your home directory using any kind of a path you'd like.
2. Create a new directory called "my_directory" in your home directory using an absolute path.
3. Navigate into "my_directory" using a relative path.
4. Create a new file called "my_file.txt" in "my_directory" using a relative path.
5. Move "my_file.txt" to your home directory using an absolute path.
6. Delete "my_directory" using a relative path.
7. Create a new directory called "my_folder" in your home directory using an absolute path.
8. Navigate into "my_folder" using a relative path.
9. Create a new file called "my_text.txt" in "my_folder" using an absolute path.
10. Move "my_text.txt" to your home directory using a relative path.
11. Delete "my_folder" using an absolute path.
12. Create a new directory called "my_new_directory" in your home directory using an absolute path.
13. Navigate into "my_new_directory" using a relative path.
14. Create a new file called "my_new_file.txt" in "my_new_directory" using an absolute path.
15. Move "my_new_file.txt" to your home directory using a relative path.

Good luck!
