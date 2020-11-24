##### [back-home](https://mhd22.github.io/301-reading-notes/)



# Read: 09 - Refactoring

## Concepts of Functional Programming in Javascript

* Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and 

## pure functions

* So how do we know if a function is pure or not? Here is a very strict definition of purity:

  * It returns the same result if given the same arguments (it is also referred as deterministic)
  * It does not cause any observable side effects

***Example about impure functions:***
* Reading Files
* Random number generation

***Examples of observable side effects include modifying a global object or a parameter passed by reference.***

## Pure functions benefits:

* The code’s definitely easier to test. We don’t need to mock anything.
* So we can unit test pure functions with different contexts:
  * Given a parameter A → expect the function to return value B
  * Given a parameter C → expect the function to return value D

## Immutability

* **Unchanging over time or unable to be changed.**

* When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

* In Javascript we commonly use the for loop. This next for statement has some mutable variables.
* For each iteration, we are changing the i and the sumOfValue state.

### But how do we handle mutability in iteration? `Recursion`!

```
let list = [1, 2, 3, 4, 5];
let accumulator = 0;

function sum(list, accumulator) {
  if (list.length == 0) {
    return accumulator;
  }

  return sum(list.slice(1), accumulator + list[0]);
}

sum(list, accumulator); // 15
list; // [1, 2, 3, 4, 5]
accumulator; // 0
```



#### _____________________________________________



### This file wrote by [Mohamad Saad Eddin](https://github.com/MHD22).
***you can visit my profile and follow me.***
### ______________________________________________


###### Thanks for your time, I hope that you have enjoyed.