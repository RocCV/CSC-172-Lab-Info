# Basic Command Lines
This README file will teach you the basic command line usage for macOS/Linux. Note that this guide is not comprehensive; if you are interested in more commands, you should search them on google.


## The Basics
After opening your terminal, you should see a `$`. You can then type any command after the dollar sign. The home directory is indicated by `~`.


### Directories
```bash
$ cd [folder]
```
This will **change the current directory** to `[folder]`. For example, if you type `$ cd Desktop`, you will navigate to the `Desktop` directory.

*Note*: if you type `$ cd` in any directory, you will go back to your home directory.

*Quick tip*: you can drag a folder to your terminal, and the terminal will copy the folder path to the command line.

---

```bash
$ pwd
```
This will **print out the current working directory**. For example, if you type `$ pwd` in the home  directory, you should see something like `/Users/[YourName]`.

---

```bash
$ ls
```
This will **list out all the files and folders in the current directory**. You can also add `-l` to list out files/folders in details, or `-a` to list out files/folders and hidden files/folders.

---

```bash
$ mkdir [folder_name]
```
This will **create a new folder named 'folder_name'**. For example, if you type `$ mkdir test` in your Desktop directory,  you will create a folder named 'test' in the Desktop.

---

### Files
```bash
$ touch [file_name]
```
This will **create a new file named 'file_name'**. For example, if you type `$ touch hello.txt` in your Desktop directory, you will create a file named 'hello.txt' in the Desktop.

---

```bash
$ open [file_name]
```
This will **open the file whose name is 'file_name'**.

---

```bash
$ cat [file_name]
```
This will **display the file whose name is 'file_name' in terminal**.

---

### Miscellaneous
```bash
$ clear
```
This will **clear the terminal screen**.


## Java
Now, you should have some basic understanding of how to use the command line. Here, I will show you how to run java program in terminal.

First, you should navigate to the directory that contains java file(s). If you use `Eclipse` to write java program, the java file(s) should be in the `src` folder. After that, type
```bash
$ javac [java file name]                  # this will create a .class file
$ java [java file name without .java]     # this will run the java program
```
Example:
```bash
$ javac Main.java
$ java Main
```
The `javac` command will take `Main.java` as input and output a `Main.class`, which is in bytecode, and the `java` command will execute that bytecode.

*Quick tip*: You can type `javac *.java` to create all .class files at once.

In addition, you can also add parameters after the `java` command. For instance, in Lab4, you can type
```bash
$ java DNAList <arraysize> <commandfile>    # without the '<' and '>'
```
Inside the main method, you can use `args[0]` to access the `arraysize` and `args[1]` to access the `commandfile`.

If you want to terminate a java program, like a running `GUI` or an `infinite loop`, you can press `ctrl+c` to terminate the program.
