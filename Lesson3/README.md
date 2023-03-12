# Lesson 3: Input and Output
In this lesson, we will cover input and output in C programming.

## Standard Input and Output
In C, the `stdio.h` header file provides functions for standard input and output. The `printf()` function is used for output and the `scanf()` function is used for input.

Here is an example of using `printf()` to output a string:

```c
printf("Hello, World!\n");

```
And here is an example of using `scanf()` to read an integer from the user:

```c
int num;
scanf("%d", &num);

```

The `%d` is a format specifier that tells `scanf()` to read an integer, and the `&` symbol is used to obtain the address of the variable `num`.

## File Input and Output
In addition to standard input and output, C also provides functions for file input and output. The `stdio.h` header file provides functions such as `fopen()`, `fclose()`, `fscanf()`, and `fprintf()`.

Here is an example of opening a file for writing and writing a string to it:

```c
#include <stdio.h>

int main() {
    FILE *fp;
    char str[] = "This is a test";
    
    fp = fopen("test.txt", "w");
    fprintf(fp, "%s", str);
    fclose(fp);
    
    return 0;
}

```

In this example, `fopen()` is used to open a file named `"test.txt"` for writing. The `"w"` argument specifies that the file should be opened for writing, and if the file doesn't exist it will be created. The `fprintf()` function is used to write the string `str` to the file, and the `fclose()` function is used to close the file.

Here is an example of opening a file for reading and reading a string from it:

```c
#include <stdio.h>

int main() {
    FILE *fp;
    char str[50];
    
    fp = fopen("test.txt", "r");
    fscanf(fp, "%s", str);
    fclose(fp);
    
    printf("%s\n", str);
    
    return 0;
}

```

In this example, `fopen()` is used to open the file `"test.txt"` for reading. The `"r"` argument specifies that the file should be opened for reading. The `fscanf()` function is used to read a string from the file into the `str` array, and the `fclose()` function is used to close the file. Finally, `printf()` is used to output the string to the console.

