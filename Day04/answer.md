# Day 4 Task: Basic Linux Shell Scripting for DevOps Engineers

## What is Kernel?

The kernel is a computer program that is the core of a computer’s operating system, with complete control over everything in the system.

## What is Shell?

A shell is a special user program that provides an interface for users to interact with operating system services. It accepts human-readable commands from users and converts them into instructions that the kernel can understand. The shell is a command language interpreter that executes commands read from input devices such as keyboards or from files. It starts when the user logs in or opens a terminal.

## What is Linux Shell Scripting?

Linux shell scripting involves writing programs (scripts) that can be run by a Linux shell, such as bash (Bourne Again Shell). These scripts automate tasks, perform system administration tasks, and facilitate the interaction between users and the operating system.

**Tasks:**
- Explain in your own words and with examples what Shell Scripting means for DevOps.
## ANS :- 
# Shell Scripting in DevOps

Shell scripting in DevOps refers to the use of scripts written in a shell (such as Bash, Zsh, or PowerShell) to automate routine tasks in managing and deploying applications or infrastructure. It's a powerful tool for automating workflows, reducing manual intervention, and ensuring consistency across environments.

## Why it's important in DevOps:
- **Automation**: Tasks like setting up servers, deploying applications, or managing files can be automated. This reduces human error and speeds up processes.
- **Efficiency**: Routine tasks that might take time if done manually can be run quickly via scripts.
- **Consistency**: Scripts ensure that tasks are done the same way every time, reducing the risk of configuration drift.

- What is `#!/bin/bash`? Can we write `#!/bin/sh` as well?
## ANS:- 
# Understanding `#!/bin/bash` and `#!/bin/sh`

In shell scripting, **`#!/bin/bash`** and **`#!/bin/sh`** are shebangs that tell the system which shell interpreter to use.

- **`#!/bin/bash`**: Specifies the Bash shell, offering advanced features like arrays, `[[ ... ]]` for conditions, and extended string manipulation.
- **`#!/bin/sh`**: Refers to the Bourne shell, or in modern systems, a faster alternative like Dash, with fewer features but greater portability.

## When to Use Which:
- Use **`#!/bin/bash`** if you need Bash-specific features or are working in a Linux environment where Bash is the default shell.
- Use **`#!/bin/sh`** if you're aiming for portability across various UNIX-like systems or your script doesn't need advanced Bash features.

- Write a Shell Script that prints `I will complete #90DaysOfDevOps challenge`.
## ANS 
  ![Image](Day04/image/task01.png)




