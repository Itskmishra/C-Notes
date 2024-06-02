```c
/*
A very basic calculator in c which teach's us about variables, conditions, and user input.
*/

#include <stdio.h>

int main () {
  // define variable to store values
  int valueA;
  int valueB;
  char op;
  // take input for the variables
  printf("Enter first value:");
  scanf("%d", &valueA);

  printf("Operator:");
  scanf(" %c", &op);

  printf("Enter second value:");
  scanf("%d", &valueB); 

  // variable to store result
  int result;
  // using if to check operator and perform action based on it.
  if(op == '+'){
    result = valueA + valueB;
  }else if (op == '-'){
    result = valueA - valueB;
  }else if (op == '*'){
    result = valueA * valueB;
  }else if (op == '/'){
    result = valueA / valueB;
  }else{
    printf("You entered something wrong!");
    return 1;
  }

  printf("Result: %d \n", result);
  return 0;
}
```
