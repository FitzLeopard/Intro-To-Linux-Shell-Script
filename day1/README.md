## Notes on Day 1

### How to write and execute a script

1. Edit the script with an editor like **Vim, Emacs or nano**

2. Make the script executable by using the following command:

   `chmod +x Filename` or `chomod +rx Filename`

3. Execute the script by `./Filename`
  

### Notes on different steps

- Step 2:

  The difference between these two commands is the `r` after the `+`.

  Actually, the first one gives the script execute permission.

  The second on gives the script both execute and read permission.

  But in many system, the read permission of the script has already been granted to the user.

  - Reason for the difference:

    We need both the read and execute permission to execute a script because the command are read in from the script.

- Check the permission granted to the user by `ls -l Filename`

  We will get something like `-rwxr-xr-x` in the first section of the output. The very first character `-` indicates the type of the file and it will be `d` if it is a directory.

  The next nine characters can be divided into three section, three characters per section, standing for 

  1. The permission granted to the owner of the file
  2. The permission granted to the group of the file
  3. The permission granted to other users

  where `r` for read, `w` for write  and `x` for execute.

  The third section of the output indicates the owner and the fourth indicates the group.

