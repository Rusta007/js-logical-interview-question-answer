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

## some questions related to the length property of arrays

Easy: Task 1
#### 1. Write a program that takes an array of numbers as input and prints the total number of elements in the array.

```
function print(arr){
    console.log(arr.length)
}
print([1,2,3,4,5,6])
```

Medium: Task 2
#### 2. Write a function that takes an array of strings as input and prints each string along with its length.

```
function task2(arr){
    for(let i = 0; i< arr.length; i++){
        console.log(i ,arr[i])
    }
}

const arr = ["abc", "bcd", "def"]
task2(arr)
```

Hard: Task 3
#### 3. Write a program that takes two arrays as input and checks if they have the same length. If they do, print "Arrays are of equal length," otherwise, print "Arrays are of different lengths."

```
function taskThird(arr1, arr2){
    if(arr1.length === arr2.length){
        console.log("Arrays are of equal length")
    }else{
          console.log("Arrays are of different lengths")
    }
}
const arr1 = [1,2,3,4]
const arr2 = [1,2,3,4,5]
taskThird(arr1, arr2)
```

Easy: Task 1
#### 1. Write a program that takes two arrays of numbers as input and uses the concat method to concatenate them. Print the resulting array.

```
function taskFirst(arr1, arr2){
    console.log(arr1.concat(arr2))
}
const arr1 = [1, 2, 3, 4];
const arr2 = [1, 2, 3, 4];
taskFirst(arr1, arr2);

```

Medium: Task 2
#### 2. Write a function that takes two arrays of strings as input and returns a new array containing the strings from both arrays, but without any duplicates.

```
function taskSecond(arr1, arr2){
    const uniqueArr = [...new Set(arr1.concat(arr2))];
    console.log(uniqueArr);
}

const arr1 = ["abc", "cde", "efg"];
const arr2 = ["abc", "ghi"];
taskSecond(arr1, arr2);

```

Hard: Task 3
#### 3. Write a program that takes three arrays of different data types (e.g., numbers, strings, and booleans) and uses the concat method to merge them into a single array. Ensure that the resulting array maintains the original order of elements.

```
function taskThird(arr1, arr2, arr3){
    const arr = arr1.concat(arr2);
    console.log(arr.concat(arr3));
}

const arr1 = [1, 2, 3, 4];
const arr2 = ["abc", "cde", "efg"];
const arr3 = [true, false];
taskThird(arr1, arr2, arr3);

```














