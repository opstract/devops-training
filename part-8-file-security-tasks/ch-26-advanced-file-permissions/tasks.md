# Advanced File Permissions Tasks:
1.
- **Set up** a directory, owned by the group **sports.**
- Members of the sports group should be able to create files in this directory.
- All files created in this directory should be group-owned by the **sports** group.
- **Users** should be able to delete only their own **user-owned** files.
- **Test** that this works!
2. **Verify** the permissions on **/usr/bin/passwd**. Remove the **setuid**, then **try** changing your password as a **normal user.** **Reset** the permissions back and try again.
3. Read about file attributes in the man page of **chattr** and **lsattr**. Try setting the i attribute on a file and test that it works.
