# File Permissions in Linux

To view the permissions of a file, you can run:
```
ls -l file.txt
```
## Read
Read the contents of a file.
You can view the contents of file.txt by running the command:
```
cat file.txt
```
To deny read permissions for the file, you can run:
```
chmod u-r file.txt
```
This command disables the read permission for the particular file.

To enable back read permissions for the file, you can run the command:
```
chmod u+r file.txt
```

## Write
Modify the contents of a file

You can modify the contents of the file by using a text editor such as nano:

```
nano file.txt
```

To deny writing permissions, you can run the command:
```
chmod u-w file.txt
```

You can open the file using a text editor, however, modifying you cannot modify the file.

To re-enable writing permissions for the file, you can run:
```
chmod u+w file.txt
```
## Execute
The execute permission is only valid for files that are executable.

A regular file is not executable.

You can create a simple c program:

```
/write.c

#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

You can also make the file executable by compiling it using the following command:
```
gcc -o write write.c
```

The c program can now be executed. To view the output, you can run:
```
./write
```

You can deny execute permissions by running the command:
```
chmod u-x write
```

To re-grant executing permissions, you can run:
```
chmod u+x write
```

This makes the file executable once again