## **1. Generate a random number between 1 and 100**

**Question:**
Write a program to generate a random number between 1 and 100.

**Code:**

```js
const randomNumber = Math.floor(Math.random() * 100) + 1;
```

**Explanation:**
`Math.random()` generates a value between 0 and 1.
Multiplying by 100 gives 0–99, and adding 1 avoids 0.

---

## **2. Check even or odd**

**Question:**
Write a program to check whether a number is even or odd.

**Code:**

```js
function checkEvenOdd(num) {
  return num % 2 === 0 ? "Even" : "Odd";
}
```

**Explanation:**
If a number is divisible by 2 with no remainder, it is even.

---

## **3. Reverse a string**

**Question:**
Write a program to reverse a given string.

**Code:**

```js
const str = "hello";
const reversed = str.split("").reverse().join("");
```

**Explanation:**
The string is converted to an array, reversed, and joined back.

---

## **4. Palindrome check**

**Question:**
Write a program to check whether a string is a palindrome.

**Code:**

```js
function isPalindrome(str) {
  return str === str.split("").reverse().join("");
}
```

**Explanation:**
A palindrome reads the same forward and backward.

---

## **5. Find the largest number in an array**

**Question:**
Write a program to find the largest number in an array.

**Code:**

```js
const arr = [10, 45, 22];
const largest = Math.max(...arr);
```

**Explanation:**
Spread operator passes array values to `Math.max()`.

---

## **6. Remove duplicate elements**

**Question:**
Write a program to remove duplicates from an array.

**Code:**

```js
const uniqueArray = [...new Set([1, 2, 2, 3])];
```

**Explanation:**
`Set` automatically removes duplicate values.

---

## **7. Count vowels in a string**

**Question:**
Write a program to count vowels in a string.

**Code:**

```js
function countVowels(str) {
  return str.match(/[aeiou]/gi)?.length || 0;
}
```

**Explanation:**
Regular expression finds vowels in the string.

---

## **8. Sum of array elements**

**Question:**
Write a program to find the sum of numbers in an array.

**Code:**

```js
const sum = [1, 2, 3].reduce((total, num) => total + num, 0);
```

**Explanation:**
`reduce()` adds all elements into a single value.

---

## **9. Sort an array**

**Question:**
Write a program to sort an array in ascending order.

**Code:**

```js
const sorted = [3, 1, 5].sort((a, b) => a - b);
```

**Explanation:**
Comparator function ensures numeric sorting.

---

## **10. Prime number check**

**Question:**
Write a program to check whether a number is prime.

**Code:**

```js
function isPrime(num) {
  if (num < 2) return false;
  for (let i = 2; i <= Math.sqrt(num); i++) {
    if (num % i === 0) return false;
  }
  return true;
}
```

**Explanation:**
A prime number has only two factors: 1 and itself.

---

## **11. Factorial of a number**

**Question:**
Write a program to find the factorial of a number.

**Code:**

```js
function factorial(n) {
  return n === 0 ? 1 : n * factorial(n - 1);
}
```

**Explanation:**
Factorial is the product of all positive integers up to the number.

---

## **12. Fibonacci series**

**Question:**
Write a program to generate Fibonacci series.

**Code:**

```js
let a = 0, b = 1;
for (let i = 0; i < 5; i++) {
  console.log(a);
  [a, b] = [b, a + b];
}
```

**Explanation:**
Each number is the sum of the previous two.

---

## **13. Merge two arrays**

**Question:**
Write a program to merge two arrays.

**Code:**

```js
const merged = [...arr1, ...arr2];
```

**Explanation:**
Spread operator joins multiple arrays.

---

## **14. Second largest number**

**Question:**
Write a program to find the second largest number in an array.

**Code:**

```js
const nums = [10, 20, 30];
const secondLargest = [...new Set(nums)].sort((a,b)=>b-a)[1];
```

**Explanation:**
Duplicates removed, array sorted, second element selected.

---

## **15. Celsius to Fahrenheit**

**Question:**
Write a program to convert Celsius to Fahrenheit.

**Code:**

```js
const fahrenheit = c => (c * 9/5) + 32;
```

**Explanation:**
Standard temperature conversion formula.

---

## **16. Check empty array**

**Question:**
Write a program to check whether an array is empty.

**Code:**

```js
const isEmpty = arr.length === 0;
```

**Explanation:**
Array length zero means empty.

---

## **17. Capitalize first letter**

**Question:**
Write a program to capitalize the first letter of a string.

**Code:**

```js
const capitalized = str[0].toUpperCase() + str.slice(1);
```

**Explanation:**
First character is uppercased, rest remains same.

---

## **18. Count words in a sentence**

**Question:**
Write a program to count words in a sentence.

**Code:**

```js
const wordCount = sentence.split(" ").length;
```

**Explanation:**
Words are separated using space.

---

## **19. Check value in array**

**Question:**
Write a program to check if a value exists in an array.

**Code:**

```js
arr.includes(5);
```

**Explanation:**
Returns `true` if value exists.

---

## **20. Generate random OTP**

**Question:**
Write a program to generate a 6-digit OTP.

**Code:**

```js
const otp = Math.floor(100000 + Math.random() * 900000);
```

**Explanation:**
Ensures OTP is always 6 digits.

---

## **21. Find object length**

**Question:**
Write a program to find the number of properties in an object.

**Code:**

```js
Object.keys(obj).length;
```

**Explanation:**
Object keys are counted.

---

## **22. React – Random number generator**

**Question:**
Create a React component to generate a random number on button click.

**Code:**

```jsx
import { useState } from "react";

function RandomNumber() {
  const [num, setNum] = useState(0);

  return (
    <button onClick={() => setNum(Math.floor(Math.random() * 100))}>
      {num}
    </button>
  );
}
```

**Explanation:**
`useState` updates the UI when button is clicked.

---



Just say it, Madina 🌸
