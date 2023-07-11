# Operating System Analysis

## #Analyze Disk Space

1. The appropriate command or tool to check the available disk space on your operating system

1) Using Windows Features 
> Settings > System > Storage

You will see a screen with various settings
To see more information about a particular category

> Apps & Features' category/

2) Using Tool

- Total Commander 
Stable file manager for Windows. It continues tradition of two-panel file managers, but is distinguished by increased convenience and functionality, supports plug-ins, has many built-in useful tools.
Find a file or disk -> F3, and you will see all information about space

- Aida64 software.
This tool for measuring your system stability through stress testing your CPU, GPU and other components like your memory and cache, can stress test and benchmark your CPU, GPU, memory, cache latency, and overall thermal performance. It also has access to your component details and can even help you with drivers if needed.


## Inodes Analysis

1. The appropriate command or tool to check the number of inodes on your operating system

In NTFS file metadata is stored in the MFT records, which is the analog of inode in Windows. Each record has its own unique ID which is the equivalent to inode number.
Generally called fileID.
We can use command to check fileID
> fsutil file queryfileid  <filename>

For my file DiskSpaceAnalysis.md, ID was 
> ID file: 0x000000000000000001920000000325df

## Resource Consumption Analysis

1. The appropriate command or tool to identify the process consuming the most RAM and CPU on your operating system.

1) Press Ctrl + Shift + Del to open the Task Manager
2) Process tab
3) There will be CPU column, that can be analyzed by sorting values from largest to smallest