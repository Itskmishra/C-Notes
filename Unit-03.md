## Variables
To create a variable, specify the **type** and assign it a **value.** You can also **declare a variable without assigning the value**, and **assign the value later**.


#### Basic Data Types

![image](https://github.com/Itskmishra/C-Notes/assets/141756495/c0b00c6a-d102-4243-9aa6-e7d09fe51105)


#### Basic Format Specifiers

![image](https://github.com/Itskmishra/C-Notes/assets/141756495/3ee4ec24-025c-4ec0-a4b0-a73c200d1aa3)


### int
stores integers (whole numbers), without decimals, such as `123` or `-123`.

```text-x-csrc
// Defining a variable with value
int my_number = 15;
// Defining a variable
int my_number2;
// Assigning the value
my_number2 = 15;
```


### float

stores floating point numbers, with decimals, such as `19.9` or `-19.9`.

```text-x-csrc
float myFloatNum = 5.1 

float myFloatNum2;
myFloatNum2 = 5.1
```


### double

stores double floating point numbers, with large values after decimals, such as `19.995165` or `-19.95165`.

```text-x-csrc
double myDoubleNum = 5.1512 

double myDoubleNum2;
myDoubleNum2 = 5.1512
```


### char

stores a single character in the variable with single quotes, such as `A` or `c`.

```text-x-csrc
char myChar = 'A'

char myChar2;
myChar2 = 'c'
```

### Constants

`const` is used to define a variable that cannot be changed after defined.

```text-x-csrc
const int myNum = 15; //This variable cannot be changed after this.
```

We cannot define a const and assign its value after. 

