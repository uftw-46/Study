## 1. What Is Bash?

**Bash** stands for **Bourne Again SHell**.

Bash is a command-line shell and scripting language commonly used on Unix/Linux systems.

It can be used to:

- Run commands
- Manage files and directories
- Process text
- Monitor processes and system resources
- Work with networks
- Manage permissions
- Automate repetitive tasks
- Write shell scripts

---

## 2. Basic Bash Commands

A Bash command generally follows:

    command [options] [arguments]

Example:

    ls -la /home

### Essential Commands

| Command | Description |
|---|---|
| `ls` | List files and directories |
| `cd` | Change directory |
| `pwd` | Show current directory |
| `echo` | Print text |
| `cat` | Display file contents |
| `cp` | Copy files/directories |
| `mv` | Move or rename files |
| `rm` | Remove files/directories |
| `touch` | Create a file |
| `mkdir` | Create a directory |
| `man` | Display command manual |
| `alias` | Create command shortcuts |

---

## 3. Navigating the File System

### Show current directory

    pwd

### List files

    ls

Detailed listing:

    ls -la

### Change directory

    cd Documents

### Go up one directory

    cd ..

### Go to home directory

    cd ~

### Go to previous directory

    cd -

---

## 4. Working With Files

### Create a file

    touch file.txt

### Display a file

    cat file.txt

### Copy a file

    cp file.txt copy.txt

### Rename or move a file

    mv old.txt new.txt

### Delete a file

    rm file.txt

### Create a directory

    mkdir projects

### Delete a directory

    rm -r projects

---

## 5. Text Processing

Important Bash text-processing commands:

- `grep`
- `awk`
- `sed`
- `cut`
- `sort`
- `head`
- `tail`

### grep

Search for text:

    grep "error" log.txt

Search recursively:

    grep -r "error" .

### awk

Extract or process columns:

    awk '{print $1}' file.txt

Multiple columns:

    awk '{print $1, $3}' data.txt

### sed

Replace text:

    sed 's/old/new/g' file.txt

### cut

Extract a column:

    cut -d "," -f 1 data.csv

### sort

Sort lines:

    sort names.txt

### head

Show the beginning of a file:

    head file.txt

Show the first 10 lines:

    head -n 10 file.txt

### tail

Show the end of a file:

    tail file.txt

Follow a changing file:

    tail -f logfile.log

---

## 6. System Monitoring

| Command | Description |
|---|---|
| `ps` | Display processes |
| `top` | Monitor running processes |
| `df` | Show disk space |
| `du` | Show file/directory usage |
| `free` | Show memory usage |
| `kill` | Terminate a process |
| `uptime` | Show system uptime |

### Processes

    ps

    ps aux

### Monitor processes

    top

### Disk space

    df -h

### Directory size

    du -sh .

### Memory

    free -h

### System uptime

    uptime

### Kill a process

    kill PID

---

## 7. Networking

| Command | Description |
|---|---|
| `ping` | Test network connectivity |
| `curl` | Transfer data |
| `wget` | Download files |
| `ssh` | Connect to a remote machine |
| `scp` | Copy files over SSH |
| `rsync` | Synchronize files |

### Ping

    ping example.com

### curl

    curl https://example.com

### Download with wget

    wget https://example.com/file.zip

### SSH

    ssh user@server

### Copy a file with SCP

    scp file.txt user@server:/path/

---

## 8. Compression and Archives

### ZIP

Create a ZIP archive:

    zip archive.zip file.txt

Extract a ZIP archive:

    unzip archive.zip

### TAR

Create a TAR archive:

    tar -cf archive.tar folder/

Extract:

    tar -xf archive.tar

Create a compressed TAR archive:

    tar -czf archive.tar.gz folder/

Extract:

    tar -xzf archive.tar.gz

---

## 9. File Permissions

Linux permissions control who can:

- Read
- Write
- Execute

There are three main permission groups:

- Owner
- Group
- Others

Permission symbols:

- `r` = read
- `w` = write
- `x` = execute

### chmod

Make a script executable:

    chmod +x script.sh

Set permissions:

    chmod 755 script.sh

### chown

Change file owner:

    chown user file.txt

### chgrp

Change group:

    chgrp group file.txt

---

## 10. Bash Scripts

A Bash script is a file containing Bash commands.

Example:

    #!/bin/bash

    echo "Hello, World!"

Save it as:

    hello.sh

Make it executable:

    chmod +x hello.sh

Run it:

    ./hello.sh

### Shebang

The first line:

    #!/bin/bash

is called the **shebang**.

It specifies which interpreter should execute the script.

---

## 11. Variables

Variables store information.

Create a variable:

    name="Alice"

Use the variable:

    echo "$name"

### Important Rule

Do not put spaces around `=`.

Correct:

    name="Alice"

Incorrect:

    name = "Alice"

### Numbers

    age=25

### Command substitution

Store command output:

    current_dir=$(pwd)

Then:

    echo "$current_dir"

---

## 12. Environment Variables

Environment variables are available to processes and programs.

Common environment variables:

- `$HOME`
- `$USER`
- `$PATH`
- `$SHELL`
- `$PWD`

Example:

    echo "$HOME"

View all environment variables:

    env

---

## 13. Operators

### Arithmetic Operators

| Operator | Meaning |
|---|---|
| `+` | Addition |
| `-` | Subtraction |
| `*` | Multiplication |
| `/` | Division |
| `%` | Modulo |

Example:

    a=10
    b=5

    echo $((a + b))
    echo $((a - b))
    echo $((a * b))
    echo $((a / b))
    echo $((a % b))

### Numeric Comparison Operators

| Operator | Meaning |
|---|---|
| `-eq` | Equal |
| `-ne` | Not equal |
| `-gt` | Greater than |
| `-lt` | Less than |
| `-ge` | Greater than or equal |
| `-le` | Less than or equal |

Example:

    if [ "$age" -ge 18 ]; then
        echo "Adult"
    fi

---

## 14. Conditions

Conditions allow scripts to make decisions.

Basic structure:

    if [ condition ]; then
        commands
    elif [ another_condition ]; then
        commands
    else
        commands
    fi

Example:

    age=20

    if [ "$age" -ge 18 ]; then
        echo "Adult"
    else
        echo "Minor"
    fi

---

## 15. String Comparisons

Example:

    name="Alice"

    if [ "$name" = "Alice" ]; then
        echo "Hello Alice"
    fi

Common string operators:

| Operator | Meaning |
|---|---|
| `=` | Equal |
| `!=` | Not equal |
| `-z` | String is empty |
| `-n` | String is not empty |

Example:

    if [ -z "$name" ]; then
        echo "Name is empty"
    fi

---

## 16. File Tests

Bash can check files and directories.

| Test | Meaning |
|---|---|
| `-f` | File exists |
| `-d` | Directory exists |
| `-e` | Path exists |
| `-r` | Readable |
| `-w` | Writable |
| `-x` | Executable |

Example:

    if [ -f "file.txt" ]; then
        echo "File exists"
    fi

Directory example:

    if [ -d "projects" ]; then
        echo "Directory exists"
    fi

---

## 17. Loops

Loops repeat commands.

### for Loop

    for item in apple banana orange
    do
        echo "$item"
    done

### Loop through files

    for file in *.txt
    do
        echo "$file"
    done

### while Loop

    count=1

    while [ "$count" -le 5 ]
    do
        echo "$count"
        ((count++))
    done

### until Loop

    count=1

    until [ "$count" -gt 5 ]
    do
        echo "$count"
        ((count++))
    done

---

## 18. Loop Control

### break

Stops a loop:

    for i in {1..10}
    do
        if [ "$i" -eq 5 ]; then
            break
        fi

        echo "$i"
    done

### continue

Skips the current iteration:

    for i in {1..5}
    do
        if [ "$i" -eq 3 ]; then
            continue
        fi

        echo "$i"
    done

---

## 19. Functions

Functions group commands into reusable blocks.

Define a function:

    greet() {
        echo "Hello!"
    }

Call it:

    greet

### Function Arguments

    greet() {
        echo "Hello, $1!"
    }

    greet "Alice"

### Special Parameters

| Parameter | Meaning |
|---|---|
| `$0` | Script/function name |
| `$1` | First argument |
| `$2` | Second argument |
| `$#` | Number of arguments |
| `$@` | All arguments |

---

## 20. Arrays

Arrays store multiple values.

Create an array:

    fruits=("apple" "banana" "orange")

Access an element:

    echo "${fruits[0]}"

Get all elements:

    echo "${fruits[@]}"

Get number of elements:

    echo "${#fruits[@]}"

Loop through an array:

    for fruit in "${fruits[@]}"
    do
        echo "$fruit"
    done

---

## 21. User Input

Use `read` to receive input.

    read -p "Enter your name: " name

    echo "Hello, $name!"

Example:

    #!/bin/bash

    read -p "Enter your age: " age

    echo "You are $age years old."

---

## 22. Command-Line Arguments

Scripts can receive arguments from the command line.

Example script:

    #!/bin/bash

    echo "Hello, $1!"

Run:

    ./hello.sh Alice

Output:

    Hello, Alice!

Important parameters:

| Parameter | Meaning |
|---|---|
| `$0` | Script name |
| `$1` | First argument |
| `$2` | Second argument |
| `$#` | Number of arguments |
| `$@` | All arguments |
| `$?` | Exit status of last command |

---

## 23. Exit Status

Commands return an exit status.

Usually:

- `0` = Success
- Non-zero = Failure/Error

Check the previous command:

    echo $?

Example:

    ls file.txt

    if [ $? -eq 0 ]; then
        echo "Command succeeded"
    else
        echo "Command failed"
    fi

---

## 24. Pipes

A pipe `|` sends the output of one command to another.

Example:

    ls | grep ".txt"

Another example:

    ps aux | grep "bash"

Concept:

    Command 1
        |
        v
      Output
        |
        v
    Command 2

Pipes are one of the most important Bash concepts.

---

## 25. Redirection

### Output to a file

    echo "Hello" > file.txt

`>` overwrites the file.

### Append to a file

    echo "Another line" >> file.txt

`>>` appends to the file.

### Input redirection

    command < file.txt

---

## 26. Standard Streams

Bash commonly works with three standard streams:

| Stream | Meaning |
|---|---|
| `stdin` | Standard input |
| `stdout` | Standard output |
| `stderr` | Standard error |

Redirect errors:

    command 2> errors.txt

Redirect output and errors:

    command > output.txt 2>&1

---

## 27. Command Chaining

### `;`

Run commands regardless of success:

    command1; command2

### `&&`

Run the second command only if the first succeeds:

    command1 && command2

### `||`

Run the second command only if the first fails:

    command1 || command2

Example:

    mkdir backup && echo "Backup directory created"

---

## 28. Quotes

### Double Quotes

Variables are expanded:

    name="Alice"

    echo "Hello $name"

Output:

    Hello Alice

### Single Quotes

Variables are not expanded:

    echo 'Hello $name'

Output:

    Hello $name

Use quotes around variables when appropriate:

    echo "$name"

This helps preserve spaces and special characters.

---

## 29. Wildcards

Bash supports pattern matching.

### `*`

Matches multiple characters:

    ls *.txt

### `?`

Matches one character:

    ls file?.txt

### `[]`

Matches characters from a set:

    ls file[123].txt

---

## 30. Command History

Show command history:

    history

Run the previous command:

    !!

Search command history:

    Ctrl + R

---

## 31. Aliases

Create a shortcut:

    alias ll='ls -la'

Then:

    ll

Remove an alias:

    unalias ll

---

## 32. Cron

**Cron** allows commands and scripts to run automatically at scheduled times.

Cron format:

    minute hour day-of-month month day-of-week command

Example:

    0 2 * * * /home/user/backup.sh

Common uses:

- Backups
- Log cleanup
- Reports
- System maintenance
- Scheduled scripts

---

## 33. Practical Bash Script

Simple backup script:

    #!/bin/bash

    SOURCE="$HOME/Documents"
    BACKUP="$HOME/backup"

    mkdir -p "$BACKUP"

    cp -r "$SOURCE" "$BACKUP"

    echo "Backup complete!"

This demonstrates:

- Shebang
- Variables
- `$HOME`
- Directory creation
- File copying
- Commands
- Output

---

## 34. Complete Example

    #!/bin/bash

    read -p "Enter your name: " name

    if [ -z "$name" ]; then
        echo "You did not enter a name."
        exit 1
    fi

    echo "Hello, $name!"

    for file in *.txt
    do
        echo "Found: $file"
    done

This combines:

- User input
- Variables
- Conditions
- Exit codes
- Loops
- File patterns

---

# 35. Bash Cheat Sheet

## Navigation

    pwd
    ls
    ls -la
    cd directory
    cd ..
    cd ~
    cd -

## Files

    touch file.txt
    cat file.txt
    cp file.txt copy.txt
    mv file.txt new.txt
    rm file.txt

## Directories

    mkdir directory
    mkdir -p path/to/directory
    rm -r directory

## Text

    grep "text" file.txt
    awk '{print $1}' file.txt
    sed 's/old/new/g' file.txt
    cut -d "," -f 1 file.csv
    sort file.txt
    head file.txt
    tail file.txt

## Processes

    ps
    ps aux
    top
    kill PID

## Disk

    df -h
    du -sh .

## Memory

    free -h

## Networking

    ping example.com
    curl https://example.com
    wget https://example.com/file
    ssh user@server
    scp file user@server:/path/

## Permissions

    chmod +x script.sh
    chmod 755 script.sh
    chown user file
    chgrp group file

## Variables

    name="Alice"
    echo "$name"

## Conditions

    if [ "$x" -gt 10 ]; then
        echo "Greater than 10"
    fi

## Loops

    for item in one two three
    do
        echo "$item"
    done

## Functions

    greet() {
        echo "Hello!"
    }

    greet

## Arrays

    items=("one" "two" "three")

    echo "${items[0]}"
    echo "${items[@]}"

## Pipes

    command1 | command2

## Redirection

    command > output.txt
    command >> output.txt
    command 2> errors.txt

## Command Chaining

    command1 && command2
    command1 || command2
    command1; command2

---

# 36. Bash Learning Path

Recommended order:

1. Learn what Bash and the terminal are
2. Learn basic commands
3. Learn file and directory navigation
4. Learn file manipulation
5. Learn pipes and redirection
6. Learn text-processing commands
7. Learn processes and system monitoring
8. Learn networking commands
9. Learn permissions
10. Write basic Bash scripts
11. Learn variables
12. Learn operators
13. Learn conditions
14. Learn loops
15. Learn functions
16. Learn arrays
17. Learn command-line arguments
18. Learn exit codes
19. Learn cron
20. Build automation projects

---

# 37. Key Concepts to Master

## Commands

    ls
    cd
    cp
    mv
    rm

## Pipes

    command1 | command2

## Redirection

    command > file.txt

## Variables

    name="Alice"
    echo "$name"

## Conditions

    if [ condition ]; then
        ...
    fi

## Loops

    for item in ...
    do
        ...
    done

## Functions

    function_name() {
        ...
    }

## Arguments

    $1
    $2
    $@

## Exit Codes

    $?

## Permissions

    chmod +x script.sh

## Automation

    Bash Script + Cron = Scheduled Automation

---

# 38. Final Summary

Bash is a powerful tool for:

- Command-line work
- Linux administration
- File management
- Text processing
- System monitoring
- Networking
- Automation
- Scripting

The goal is not to memorize every command.

Instead, learn how to **combine simple commands into useful workflows**.

The core Bash progression is:

    Commands
       ↓
    Pipes & Redirection
       ↓
    Variables
       ↓
    Conditions
       ↓
    Loops
       ↓
    Functions
       ↓
    Scripts
       ↓
    Automation

> **Bash mindset:**
>
> **Command → Combine → Script → Automate**