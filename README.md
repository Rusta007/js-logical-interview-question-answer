# js-logical-interview-question-answer

Easy: Task 1
#### 1. Write a program that prints the numbers from 1 to 5 using a for loop.

```
function printNumber(n){
    for(let i = 1; i<= n; i++){
        console.log(i)
    }
}
printNumber(5)
```

Medium: Task 2
#### 2. Write a program that calculates and prints the factorial of a given number using a for loop. For example, if the input is 5, the output should be 120 (5! = 5 x 4 x 3 x 2 x 1).

```
function factorialNumber(n){
    // console.log(n)
    let multiply = 1
    for(let i = 1; i<=n; i++){
        multiply *= i
    }
        console.log(multiply)
}
factorialNumber(5)
```

Hard: Task 3
#### 3. Write a program that generates the first 10 numbers in the Fibonacci sequence using a for loop. The Fibonacci sequence starts with 0 and 1, and each subsequent number is the sum of the two preceding ones (0, 1, 1, 2, 3, 5, 8, 13, 21, 34).

```
function generateFibonacci(n) {
  let fibArray = [0, 1];

  for (let i = 2; i < n; i++) {
    fibArray[i] = fibArray[i - 1] + fibArray[i - 2];
  }

  return fibArray;
}

const fibonacciSequence = generateFibonacci(10);
console.log("Fibonacci Sequence:", fibonacciSequence);
```

