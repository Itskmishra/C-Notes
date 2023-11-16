# User Input

To get **user input**, We can use the `scanf()` function. The `scanf()` function takes two arguments: the format specifier of the variable (`%d` in the example above) and the reference operator (`&myNum`), which stores the memory address of the variable.

```text-x-csrc
int myNum;

printf("Type a number: \n");
// Get and save the number the user types
scanf("%d", &myNum);
// print the input value on the screen.
printf("Your number is: %d", myNum);
```

We can also take multiple inputs like char, number, and more.

```text-x-csrc
int myNum;
char myChar;

printf("Type a number AND a character and press enter: \n");

// Get and save the number AND character the user types
scanf("%d %c", &myNum, &myChar);

// Print the number
printf("Your number is: %d\n", myNum);

// Print the character
printf("Your character is: %c\n", myChar);
```

We can also take a string as input.

```text-x-csrc
// Create a string
char firstName[30];

// Ask the user to input some text
printf("Enter your first name: \n");

// Get and save the text
scanf("%s", firstName);

// Output the text
printf("Hello %s", firstName);
```

When taking input as a string we must specify the size of the string/array. And we don't have to use the reference operator(&).

However, the `scanf()` function has some limitations. it considers space (whitespace, tabs, etc) as a terminating character, which means that it can only display a single word (even if you type many words). That's why, when working with strings, we often use the `fgets()` function to **read a line of text**. In `fgets()` we must include the following arguments: the name of the string variable, `sizeof`(_string\_name_), and `stdin`:

```text-x-csrc
char fullName[30];

printf("Type your full name: \n");
fgets(fullName, sizeof(fullName), stdin);

printf("Hello %s", fullName);

// Type your full name: John Doe
// Hello John Doe
```
