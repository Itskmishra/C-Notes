# Array 

Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value. To create an array, define the data type (like `int`) and specify the name of the array followed by **square brackets \[\]**.

We can only store data of a certain type in an array that is defined for that type. int array can store int values only.

```text-x-csrc
int myNumbers[] = {1,2,3,4,5,6};
```

To access an array element, refer to its **index number**.

```text-x-csrc
int myNumbers[] = {25, 50, 75, 100};
printf("%d", myNumbers[0]);

// Outputs 25
```

Changing value can be done using the index number

```text-x-csrc
myNumbers[0] = 33;
```

We can define the size of an array to store a specific number of values.

```text-x-csrc
// Declare an array of four integers:
int myNumbers[4];
// Add elements
myNumbers[0] = 25;
myNumbers[1] = 50;
myNumbers[2] = 75;
myNumbers[3] = 100;
```

## Multidimensional Array

A multidimensional array is basically an array of arrays.

### Two-Dimensional Arrays

A 2D array is also known as a matrix (a table of rows and columns). To create a 2D array of integers,

```text-x-csrc
int matrix[2][3] = { {1, 4, 2}, {3, 6, 8} };

// 2D array
1  4  2
3  6  8
```

To access an array element, refer to its **array index** and **element index** 

```text-x-csrc
int matrix[2][3] = { {1, 4, 2}, {3, 6, 8} };
// access the first value of the first array in the matrix.
matrix[0][0] = 9;
```
