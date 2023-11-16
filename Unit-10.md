# Strings 
Strings are used for storing text/characters. Unlike many other programming languages, C does not have a **String type** to easily create string variables. Instead, you must use the `char` type and create an of characters to make a string in C.

## Method 1: 
```text-x-csrc
char greetings[] = "Hello World!"; // a string stored in greetings array.
```

Note that you have to use double quotes (`""`). To write a string.

To output the string, you can use the `printf()` function together with the format specifier `%s` to tell C that we are now working with strings:

```text-x-csrc
char greetings[] = "Hello World!";
printf("%s", greetings);
```

All the array actions can be performed because it's an array of chars.

## Methods 2: 

We can create a string with a set of characters. 

```text-x-csrc
char greetings[] = {'H', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd', '!', '\0'};
printf("%s", greetings);
```

**Why do we include the** `**\0**` **character at the end?** This is known as the "null terminating character", and must be included when creating strings using this method. It tells C that this is the end of the string.

#### Difference between method 1 and method 2

The difference between the two ways of creating strings is that the first method is easier to write, and you do not have to include the `\0` character, as C will do it for us.

We should note that the size of both arrays is the same: They both have **13 characters** (space also counts as a character by the way), including the `\0` character.
