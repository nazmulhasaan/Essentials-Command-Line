# Essentials Terminal Commands

This guide provides a comprehensive overview of essential terminal commands. Whether you're a beginner or an experienced user, these commands will help you navigate and perform tasks efficiently in your terminal.

## Key Commands & Navigation
These keyboard shortcuts can save you time while working in the terminal:

- **Up Arrow**: Show your last command
- **Down Arrow**: Show your next command
- **Tab**: Auto-complete your command
- **Ctrl + L**: Clear the screen
- **Ctrl + C**: Cancel a command
- **Ctrl + R**: Search for a command
- **Ctrl + D**: Exit the terminal

## Manual Command
On Linux and macOS, use the `man` command to view the manual for any terminal command. For example, to learn more about the `ls` command:

```bash
man ls
```

On Windows (Git Bash), you can use the `--help` flag instead:

```bash
ls --help
```

## User & Date Commands

### `whoami`
Displays the current user:

```bash
whoami
```

### `date`
Shows the current date and time:

```bash
date
```

## File System Navigation

| Command                             | Description                                                    |
| ----------------------------------- | -------------------------------------------------------------- |
| `pwd`                               | Print working directory                                         |
| `ls`                                | List directory contents                                         |
| `ls -a`                             | List all contents, including hidden files                       |
| `ls -l`                             | List contents with details (permissions, owner, size, etc.)     |
| `ls -r`                             | List contents in reverse order                                  |
| `cd [dirname]`                      | Change directory to `[dirname]`                                 |
| `cd ~`                              | Change to home directory                                        |
| `cd ..`                             | Move to the parent directory                                    |
| `cd -`                              | Switch to the previous directory                                |
| `find [directory] -name [filename]` | Search for a file named `[filename]` in `[directory]`           |

Combine multiple flags for more detailed output, like `ls -la` to see hidden files with extra details.

## Opening Files or Folders

Open folders or files directly from the terminal based on your OS:

- **macOS**: `open [dirname]`
- **Windows**: `start [dirname]`
- **Linux**: `xdg-open [dirname]`

You can also open URLs:

```bash
open https://traversymedia.com
```

## Modifying Files & Directories

| Command                                | Description                               |
| -------------------------------------- | ----------------------------------------- |
| `mkdir [dirname]`                      | Create a new directory                    |
| `touch [filename]`                     | Create a new file                         |
| `rm [filename]`                        | Delete a file                             |
| `rm -r [dirname]`                      | Delete a directory                        |
| `rm -rf [dirname]`                     | Force delete a directory and its contents |
| `cp [source] [destination]`            | Copy a file                               |
| `mv [source] [destination]`            | Move or rename a file or directory        |

## Concatenation & Redirection

The `cat` command is useful for displaying file contents, creating new files, and appending to existing ones.

### Display File Contents

```bash
cat [filename]
```

### Create a File

```bash
cat > [filename]
```
(Type content and press `Ctrl + D` to save and exit.)

### Append to a File

```bash
cat >> [filename]
```

Use the `>` symbol to redirect output into a file:

```bash
echo "Hello World" > [filename]
```

## Viewing File Contents

- **less**: Allows scrolling through file content.
  
  ```bash
  less [filename]
  ```

- **head**: Outputs the first few lines of a file (default is 10 lines).

  ```bash
  head [filename]
  ```

- **tail**: Outputs the last few lines of a file (default is 10 lines).

  ```bash
  tail [filename]
  ```

## Search & Filter

- **grep**: Search for a text pattern within a file.

  ```bash
  grep [searchterm] [filename]
  ```

## File Search

The `find` command helps locate files or directories based on conditions.

### Example: Find a File by Name

```bash
find . -name "file-001.txt"
```

### Example: Find Empty Files

```bash
find . -empty
```

## File Compression with tar

| Command                          | Description                                      |
| --------------------------------- | ------------------------------------------------ |
| `tar czvf [archive].tar.gz [dir]` | Create a tarball (compressed archive)            |
| `tar xzvf [archive].tar.gz`       | Extract a tarball                                |
| `tar tzvf [archive]`              | View contents of a tarball                       |

## History & Shortcuts

Use `history` to view the command history, or execute a command from history by its position number:

```bash
!100
```

## Piping & Symlinks

- **Piping**: Use `|` to send the output of one command to another.

  ```bash
  find . -name "file-*" > output.txt
  ```

- **Symlink**: Create a symbolic link (shortcut to a file):

  ```bash
  ln -s [filename] [symlinkname]
  ```

---

This guide covers essential commands for efficient terminal use across Linux, macOS, and Windows (Git Bash). You can explore more advanced features as you become more comfortable with the terminal.

---
