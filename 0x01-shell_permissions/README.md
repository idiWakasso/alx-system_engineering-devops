# SHELL: Permissions

This README file provides an overview of Linux file permissions and essential commands related to permissions management. Understanding permissions is crucial for maintaining security and controlling access to files and directories within a Linux system. This document will cover the following topics:

## Commands

- `chmod`: Change file permissions.
- `sudo`: Execute commands with superuser privileges.
- `su`: Switch to another user account.
- `chown`: Change file ownership.
- `chgrp`: Change file group ownership.

## Linux File Permissions

Linux file permissions determine the level of access that users and groups have to files and directories. Permissions are divided into three sets: owner, group, and other. Each set consists of three permission types: read, write, and execute. Permissions can be represented as a single digit:

| Permission | Digit |
|------------|-------|
| No permission | 0 |
| Execute permission | 1 |
| Write permission | 2 |
| Write and execute permissions | 3 |
| Read permission | 4 |
| Read and execute permissions | 5 |
| Read and write permissions | 6 |
| Read, write, and execute permissions | 7 |

## Changing Permissions, Ownership, and Group

The `chmod` command is used to modify file permissions. The `chown` command changes the ownership of a file, and the `chgrp` command changes the group ownership of a file. Only the file owner or superuser (root) can change permissions, ownership, and group.

## Limitations of Changing Ownership

Regular users do not have permission to change the ownership of files owned by other users. Changing ownership is limited to the file owner and superuser for security reasons.

## Running Commands with Root Privileges

The `sudo` command allows users to execute commands with superuser privileges. By using `sudo`, users can perform administrative tasks without needing to switch to the root account.

## Changing User ID or Becoming Superuser

The `su` command enables a user to switch to another user account, including the superuser (root). Superuser privileges can be obtained by running commands as the root user or by using `su` to become the superuser temporarily.

Understanding and managing permissions are essential skills for effective Linux administration. By grasping the concepts and mastering the commands mentioned above, you will be able to maintain a secure and controlled environment within your Linux system.

Please refer to the relevant man pages and additional resources for more detailed information on each command and permission management in Linux.

