---
layout: single
title: SUID, SGID and Stickybit
tags: linux
---

# SUID, SGID, and Sticky Bit


SUID, SGID, and sticky bits are Linux file attributes that allow you to define special permissions on files and directories. These attributes can be set using the chmod command and have different effects on the file or directory depending on their usage.

### SUID
SUID (Set User ID) is a file attribute that allows the user who executes the file to run it with the permissions of the file's owner. This is useful when you need to give non-root users permission to perform tasks that require root privileges. For example, if you have a file owned by the root user with SUID enabled, a non-root user can execute the file with root privileges.

### SGID
SGID (Set Group ID) is a file attribute that allows files to be executed with the permissions of the group owner. When SGID is enabled on a directory, new files created in that directory inherit the group ownership of the parent directory. SGID is useful in situations where multiple users need to access files in the same directory and have the same level of access.

### Sticky bit
The sticky bit is a file attribute that can be set on directories. When set, it ensures that only the owner of a file or directory can delete or rename it, even if other users have write access to the directory. The sticky bit is often used on directories that are shared by multiple users to prevent accidental deletion or modification of files.

It's important to note that SUID, SGID, and sticky bits can introduce security risks if used improperly. For example, enabling SUID on a file that can be modified by other users can allow a malicious user to execute arbitrary code as the file's owner.

### Conclusion
In conclusion, SUID, SGID, and sticky bits are powerful Linux file attributes that allow you to set special permissions on files and directories. By using them correctly, you can provide users with the permissions they need to perform tasks while maintaining security and control over your system.  

<br/>
<br/>
