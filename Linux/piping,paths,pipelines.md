
## **1. Piping (`|`)**

**Definition:**  
Piping (`|`) in Linux is used to pass the output of one command as input to another command. This allows you to combine multiple commands into a powerful workflow.

**Syntax:**



`command1 | command2 | command3`

**How it works:**

- `command1` produces output.
- The `|` operator takes that output and "pipes" it into `command2`.
- `command2` processes the input and produces output, which can then be piped to another command.

**Examples:**

1. **Count lines in output:**
    

    
    `ls -l | wc -l`
    
    - `ls -l`: Lists files in long format.
    - `wc -l`: Counts the number of lines (i.e., the number of files).
2. **Search for a pattern in output:**
    

    
    `cat file.txt | grep "pattern"`
    
    - `cat file.txt`: Displays the content of `file.txt`.
    - `grep "pattern"`: Filters lines that contain "pattern".
3. **Sort and remove duplicates:**
    
 
    
    `cat file.txt | sort | uniq`
    
    - `sort`: Sorts the lines alphabetically.
    - `uniq`: Removes duplicate lines.

---

## **2. Understanding Paths**

Paths in Linux define the location of files and directories in the filesystem. There are two types:

### a) **Absolute Path**

- Starts from the root directory `/` and gives the complete location of a file or directory.
- Example:
    
 
    
    `/home/adminuser/funny-stuff/file.txt`
    

### b) **Relative Path**

- Starts from the current directory and points to a file or directory relative to where you are.
- Example:
    

    
    `./file.txt  # Refers to file.txt in the current directory. ../file.txt # Refers to file.txt in the parent directory.`
    

**Commands to Work with Paths:**

1. **Print Current Directory (`pwd`):**
    
    
    `pwd`
    
2. **Navigate Directories (`cd`):**
    
    bash
    
    CopyEdit
    
    `cd /path/to/directory   # Absolute path cd ../another-folder    # Relative path`
    
3. **List Files in a Directory (`ls`):**
    

    
    `ls /absolute/path ls ./relative/path`
    

---

## **3. Pipelines**

A **pipeline** is a sequence of commands connected by pipes (`|`). It's used to process data through multiple stages, where the output of one stage becomes the input of the next.

**Example of a Pipeline:**



`cat access.log | grep "ERROR" | sort | uniq -c | sort -nr`

What this does:

1. `cat access.log`: Reads the log file.
2. `grep "ERROR"`: Filters lines containing "ERROR".
3. `sort`: Sorts the filtered lines.
4. `uniq -c`: Counts occurrences of each unique line.
5. `sort -nr`: Sorts the counts in descending numerical order.
