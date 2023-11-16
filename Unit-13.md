# Functions

To create (often referred to as _declare_) our own function, specify the name of the function, followed by parentheses `()` and curly brackets `{}`:

```text-x-csrc
void myFunction() {
  // code to be executed
}
```

*   `myFunction()` is the name of the function
*   `void` means that the function does not have a return value. You will learn more about return values later in the next chapter
*   Inside the function (the body), add code that defines what the function should do

If we are returning int then we will use int to define the function and same for other types.

```text-x-csrc
// function return integer
int myFunction() {
	return 1;
}
// function return char
char myCharFun(){
	return 'a';
}
```

To call a function, write the function's name followed by two parentheses `()` and a semicolon `;` .

```text-x-csrc
// Create a function
void myFunction() {
  printf("I just got executed!");
}

int main() {
  myFunction(); // call the function
  return 0;
}
```

## Parameters and Arguments

Parameters are specified after the function name, inside the parentheses. We can add as many parameters as you want, just separate them with a comma

```text-x-csrc
returnType functionName(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

### Single Parameter 

```text-x-csrc
void myFunction(char name[]) {
  printf("Hello %s\n", name);
}

int main() {
  myFunction("Liam");
  return 0;
}
```

### Multiple Parameters

```text-x-csrc
void myFunction(char name[], int age) {
  printf("Hello %s. You are %d years old.\n", name, age);
}

int main() {
  myFunction("Liam", 3);
  return 0;
}
```

## Function Declaration and definition

A function consist of two parts:

*   **Declaration:** the function's name, return type, and parameters (if any)
*   **Definition:** the body of the function (code to be executed)

```text-x-csrc
void myFunction() { // declaration
  // the body of the function (definition)
}
```

We will often see C programs that have function declaration above `main()`, and function definition below `main()`. This will make the code better organized and easier to read:

```text-x-csrc
// Function declaration
void myFunction();

// The main method
int main() {
  myFunction();  // call the function
  return 0;
}

// Function definition
void myFunction() {
  printf("I just got executed!");
}
```

## Recursion

Recursion is the technique of making a function call itself.

Adding two numbers together is easy to do, but adding a range of numbers is more complicated. In the following example, recursion is used to add a range of numbers together by breaking it down into the simple task of adding two numbers:

```text-x-csrc
int sum(int k);

int main() {
  int result = sum(10);
  printf("%d", result);
  return 0;
}

int sum(int k) {
  if (k > 0) {
    return k + sum(k - 1);
  } else {
    return 0;
  }
} 
```
