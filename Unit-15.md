# Enums

An **enum** is a special type that represents a group of constants (unchangeable values).

```text-x-csrc
enum Level {
  LOW,
  MEDIUM,
  HIGH
}; 
```

To access the enum,  we must create a variable of it.

Inside the `main()` method, specify the `enum` keyword, followed by the name of the enum (`Level`) and then the name of the enum variable (`myVar` in this example):

```text-x-csrc
enum Level myVar; 
```

assign value to the defined enum var.

```text-x-csrc
enum Level myVar = MEDIUM; // The value must be inside the enum
```

By default, the first item (`LOW`) has the value `0`, the second (`MEDIUM`) has the value `1`, etc.

We can manually change the value of enums by  them.

```text-x-csrc
enum Level {
  LOW = 25,
  MEDIUM = 50,
  HIGH = 75
}; 
```

Note that if you assign a value to one specific item, the next items will update their numbers accordingly:

```text-x-csrc
enum Level {
  LOW = 5,
  MEDIUM, // Now 6
  HIGH // Now 7
}; 
```

**use case** : Use enums when you have values that you know aren't going to change, like month days, days, colors, deck of cards, etc.
