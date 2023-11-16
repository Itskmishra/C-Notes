## A basic "Hello, world" function in C will resemble the following code.

```text-x-csrc
#include <stdio.h>

int main() {
  printf("Hello World!");
  return 0;
} 
```

`#include <stdio.h>`   : header files library that lets us work with input and output functions, such as `printf()` . Header files add functionality to C programs.

`int main() {}`  : This is called a function. Anything inside its curly brackets `{}`  will be executed. In C the main function is the entry point of the program.

`printf()` : is a function used to output text to the screen. We can use this because we have imported stdio header file at the top. 

```text-plain
printf("Hello World!"); // this line in the code called statement.

NOTE: Every C statement ends with a semicolon ";". 
```

`return 0;` :  ends the `main()` function.
