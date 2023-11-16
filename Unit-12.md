# Memory Address

When a variable is created in C, a memory address is assigned to the variable. The memory address is the location of where the variable is stored on the computer. When we assign a value to the variable, it is stored in this memory address. To access it, use the reference operator (`&`), and the result represents where the variable is stored:

```text-x-csrc
int myAge = 43;
printf("%p", &myAge); // Outputs 0x7ffe5367e044
```

We should also note that `&myAge` is often called a "pointer". A pointer basically stores the memory address of a variable as its value. To print pointer values, we use the `%p` format specifier.

## Pointers

A **pointer** is a variable that **stores** the **memory address** of another variable as its value.  A **pointer variable** **points** to a **data type** (like `int`) of the same type, and is created with the `*` operator. 

```text-x-csrc
int myAge = 43;     // An int variable
int* ptr = &myAge;  // A pointer variable, with the name ptr, that stores the address of myAge

// Output the value of myAge (43)
printf("%d\n", myAge);

// Output the memory address of myAge (0x7ffe5367e044)
printf("%p\n", &myAge);

// Output the memory address of myAge with the pointer (0x7ffe5367e044)
printf("%p\n", ptr);
```

### Example explained

Create a pointer variable with the name `ptr`, that **points to** an `int` variable (`myAge`). Note that the type of the pointer has to match the type of the variable you're working with (`int` in our example).

Use the `&` operator to store the memory address of the `myAge` variable, and assign it to the pointer.

Now, `ptr` holds the value of `myAge`'s memory address.

## Dereference

We can also get the value of the variable the pointer points to, by using the `*` operator (the **dereference** operator):

```text-x-csrc
int myAge = 43;     // Variable declaration
int* ptr = &myAge;  // Pointer declaration

// Reference: Output the memory address of myAge with the pointer (0x7ffe5367e044)
printf("%p\n", ptr);

// Dereference: Output the value of myAge with the pointer (43)
printf("%d\n", *ptr);
```

Note that the `*` sign can be confusing here, as it does two different things in our code:

*   When used in declaration (`int* ptr`), it creates a **pointer variable**.
*   When not used in declaration, it act as a **dereference operator**.
