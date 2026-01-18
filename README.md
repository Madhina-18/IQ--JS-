Coding Questions 
---

### **1. Math.random() (1 to 10)**

**Question:**
Write a JavaScript program to generate a random number between 1 and 10. 

**Code:**

```javascript
let num = Math.floor(Math.random() * 10) + 1;
console.log(num);
```

**Output:**

```
Any number between 1 and 10
```

---

### **2. Return Keyword**

**Question:**
Write a JavaScript function that uses the `return` keyword.

**Code:**

```javascript
function getValue() {
  return 10;
}
console.log(getValue());
```

**Output:**

```
10
```

---

### **3. Ternary Operator**

**Question:**
Write a JavaScript program using the ternary operator to check even or odd.

**Code:**

```javascript
let num = 5;
let result = (num % 2 === 0) ? "Even" : "Odd";
console.log(result);
```

**Output:**

```
Odd
```

---

### **4. Loop in JavaScript**

**Question:**
Write a JavaScript program to print numbers from 1 to 10 using a loop.

**Code:**

```javascript
for (let i = 1; i <= 10; i++) {
  console.log(i);
}
```

**Output:**

```
1
2
3
4
5
6
7
8
9
10
```

---

### **5. push() Method**

**Question:**
Write a JavaScript program using `push()` to add an element to an array.

**Code:**

```javascript
let fruits = ["Apple", "Banana"];
fruits.push("Orange");
console.log(fruits);
```

**Output:**

```
["Apple", "Banana", "Orange"]
```

---

### **6. splice() Method**

**Question:**
Write a JavaScript program using `splice()` to remove an element.

**Code:**

```javascript
let nums = [1, 2, 3, 4];
nums.splice(1, 1);
console.log(nums);
```

**Output:**

```
[1, 3, 4]
```

---

### **7. Object Literals**

**Question:**
Create an object literal with name, age, and role.

**Code:**

```javascript
let student = {
  name: "Ram",
  age: 21,
  role: "Developer"
};
console.log(student);
```

**Output:**

```
{name: "Ram", age: 21, role: "Developer"}
```

---

### **8. JavaScript Event**

**Question:**
Write a JavaScript program using a click event.

**Code:**

```html
<button onclick="showMsg()">Click</button>
<script>
  function showMsg() {
    alert("Button clicked");
  }
</script>
```

**Output:**

```
Button clicked (alert)
```

---

### **9. Reverse a String**

**Question:**
Write a JavaScript program to reverse a string.

**Code:**

```javascript
let str = "hello";
let rev = str.split("").reverse().join("");
console.log(rev);
```

**Output:**

```
olleh
```

---

10 . Write a simple JavaScript program to check whether a given string is a palindrome or not.

**Answer:**

```javascript
let word = "madam";
let rev = word.split("").reverse().join("");

if (word === rev) {
  console.log("Palindrome");
} else {
  console.log("Not a Palindrome");
}
```

**Output:**

```
Palindrome
```

### **11. Arrow Function**

**Question:**
Write a JavaScript program using an **arrow function** to add two numbers.

**Answer:**

```javascript
const add = (a, b) => a + b;
console.log(add(5, 3));
```

**Output:**

```
8
```


### **12. Callback Function**

**Answer:**

```javascript
function greet(name) {
  console.log("Hello " + name);
}

function processUser(callback) {
  let userName = "Ram";
  callback(userName);
}

processUser(greet);
```

**Output:**

```
Hello Ram
```

### **13. Promise**

**Question:**
Write a simple JavaScript program using a **Promise** that resolves after 2 seconds.

**Answer:**

```javascript
let myPromise = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve("Promise Resolved!");
  }, 2000);
});

myPromise.then((message) => {
  console.log(message);
});
```

**Output (after 2 seconds):**

```
Promise Resolved!
```

### **14. Async & Await**

**Question:**
Write a JavaScript program using **async/await** to wait for a promise to resolve.

**Answer:**

```javascript
function delay(ms) {
  return new Promise((resolve) => setTimeout(() => resolve("Done!"), ms));
}

async function asyncFunction() {
  let result = await delay(2000);
  console.log(result);
}

asyncFunction();
```

**Output (after 2 seconds):**

```
Done!
```

### **15. Template Literals**

**Question:**
Write a JavaScript program using **template literals** to display a message with a name and age.

**Answer:**

```javascript
let name = "Ram";
let age = 21;

let message = `My name is ${name} and I am ${age} years old.`;
console.log(message);
```

**Output:**

```
My name is Ram and I am 21 years old.
```



