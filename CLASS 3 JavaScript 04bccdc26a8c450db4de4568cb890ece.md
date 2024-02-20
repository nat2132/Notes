# CLASS 3 JavaScript

JavaScript is a programming language commonly used for web development. It allows developers to create interactive web pages and dynamic content on websites. JavaScript can be used for tasks such as form validation, creating animations, handling user interactions, and making asynchronous requests to servers. It is supported by all modern web browsers and is an essential tool for front-end and back-end web development.

# Variables are Containers for Storing Data

JavaScript Variables can be declared in 4 ways:

- Automatically
- Using `var`
- Using `let`
- Using `const`

In this first example, `x`, `y`, and `z` are undeclared variables.

They are automatically declared when first used:

# Example

x = 5;y = 6;z = x + y;

# Note

It is considered good programming practice to always declare variables before use.

From the examples you can guess:

- x stores the value 5
- y stores the value 6
- z stores the value 11

# Example using var

var x = 5; var y = 6;var z = x + y;

In JavaScript, variables hold different kinds of data, categorized into two main types: **primitive** and **non-primitive**. Understanding the difference between these two is crucial for writing efficient and effective code.

**Primitive variables:**

- **Simple and atomic:** They represent single values like numbers, strings, booleans, null, undefined, and symbols.
- **Immutable:** Once assigned, their value cannot be directly changed. Any attempt to modify them will create a new primitive value.
- **Stored directly in memory:** They occupy a fixed amount of memory space based on their type.
- **Compared by value:** Two primitives are equal if they have the same value and type.

**Non-primitive variables:**

- **Complex and composite:** They hold references to objects like arrays, functions, and other complex data structures.
- **Mutable:** Their internal state can be changed after creation.
- **Stored as references:** They hold an address in memory pointing to the actual object, not the object itself.
- **Compared by reference:** Two non-primitives are equal if they refer to the same object in memory.

Here's a table summarizing the key differences:

| Feature | Primitive | Non-Primitive |
| --- | --- | --- |
| Type | Simple | Complex |
| Mutability | Immutable | Mutable |
| Storage | Direct value in memory | Reference to object in memory |
| Equality comparison | By value | By reference |

Understanding these differences will help you choose the right data type for your variables depending on your needs:

- Use primitives for simple data like counters, scores, or flags.
- Use non-primitives for complex data like lists, user information, or game objects.

JavaScript provides a rich set of string methods for manipulating and working with textual data. These methods cover various tasks, including:

**Accessing characters:**

- `charAt(position)`: Returns the character at the specified position.
- `charCodeAt(position)`: Returns the Unicode code point of the character at the specified position.
- `[]`: Access characters using bracket notation like `str[2]`.

**Searching and replacing:**

- `indexOf(substring)`: Returns the first index of the substring within the string.
- `lastIndexOf(substring)`: Returns the last index of the substring within the string.
- `search(regexp)`: Searches for a regular expression within the string and returns its index.
- `replace(oldValue, newValue)`: Replaces all occurrences of the old value with the new value.

**Case conversion:**

- `toUpperCase()`: Converts the string to uppercase.
- `toLowerCase()`: Converts the string to lowercase.

**Trimming whitespace:**

- `trim()`: Removes leading and trailing whitespace characters.

**Splitting and joining:**

- `split(separator)`: Splits the string into an array of substrings based on the separator.
- `join(separator)`: Joins an array of strings into a single string with the specified separator.

**Checking properties:**

- `startsWith(substring)`: Checks if the string starts with the specified substring.
- `endsWith(substring)`: Checks if the string ends with the specified substring.

**Other useful methods:**

- `length`: Returns the length of the string.
- `substring(start, end)`: Extracts a substring from the string.
- `slice(start, end)`: Similar to substring, but can take negative indices.
- `concat(str1, str2, ...)`: Concatenates multiple strings.

JavaScript has a wide range of operators to perform various tasks, making it a versatile language for manipulating data and controlling program flow. Here's a breakdown of the main types of operators:

**1. Arithmetic Operators:**

- **Basic operations:** +, -, *, /, % (modulus), ++ (increment), -- (decrement)
- **Combined assignment:** +=, -=, *=, /=, %=
- **Exponentiation:** ** (a raised to the power of b)

**2. Assignment Operators:**

- **Simple assignment:** = (assigns a value to a variable)
- **Combined assignment:** +=, -=, *=, /=, %= (combine operation with assignment)

**3. Comparison Operators:**

- **Equality:** == (loose comparison), === (strict comparison)
- **Inequality:** !=, !==
- **Relational:** <, >, <=, >=

**4. Logical Operators:**

- **AND:** && (true if both operands are true)
- **OR:** || (true if at least one operand is true)
- **NOT:** ! (negates the operand)

**5. Bitwise Operators:**

- **AND:** & (performs bitwise AND)
- **OR:** | (performs bitwise OR)
- **XOR:** ^ (performs bitwise XOR)
- **NOT:** ~ (performs bitwise NOT)
- **Shift:** <<, >> (shift bits left/right)

**6. Conditional (Ternary) Operator:**

- ?: (assigns a value based on a condition)

**7. Comma Operator:**

- , (separates expressions and evaluates them from left to right)

**8. Unary Operators:**

- **Negation:** - (negates a number)
- **Type conversion:** + (converts to number), ! (converts to boolean)

**9. String Operators:**

- (concatenates strings)

**10. Object Access Operators:**

- . (dot notation to access object properties)
- [] (bracket notation to access array elements and object properties)

These are just the main categories, and each operator has specific rules and nuances.

Arrays are a fundamental data structure in JavaScript, used for storing ordered collections of data. They offer various functionalities and methods for manipulating and accessing their elements. Here's a breakdown of key aspects of arrays in JavaScript:

**Creating Arrays:**

- **Array literal:** `const numbers = [1, 2, 3];`
- **`new Array` constructor:** `const emptyArray = new Array(5);`
- **`Array.from` method:** `const fruits = Array.from(["apple", "banana", "orange"]);`

**Accessing Elements:**

- **Bracket notation:** `const firstElement = fruits[0];`
- **`length` property:** `const arrayLength = numbers.length;`
- **`forEach` method:** `fruits.forEach(fruit => console.log(fruit));`

**Manipulating Arrays:**

- **Push and pop:** `fruits.push("mango");` and `fruits.pop();`
- **Shift and unshift:** `fruits.shift();` and `fruits.unshift("kiwi");`
- **Splice:** `fruits.splice(1, 2, "grapefruit");` (removes 2 elements at index 1 and inserts "grapefruit")
- **Slice:** `const subfruits = fruits.slice(2);` (creates a new array from index 2 onwards)
- **Sort:** `fruits.sort();` (sorts elements in ascending order)
- **Filter and map:** `const citrusFruits = fruits.filter(fruit => fruit.includes("citrus"));` and `const fruitLengths = fruits.map(fruit => fruit.length);`

**Additional Features:**

- **Multidimensional arrays:** `const matrix = [[1, 2, 3], [4, 5, 6]];`
- **Destructuring:** `const [first, second] = fruits;`
- **Spread operator:** `const allFruits = [...fruits, "papaya"];`

These are just some basic concepts. To delve deeper, you can explore specific methods and functionalities in detail through the official documentation:

- MDN Web Docs - Array Object: [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array): [https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array](https://developer.mozilla.org/en-US/%3C1%3Edocs/Web/JavaScript/Reference/Global_Objects/Array)
- W3Schools - JavaScript Arrays: [https://www.w3schools.com/js/js_arrays.asp](https://www.w3schools.com/js/js_arrays.asp):[https://www.w3schools.com/js/js_arrays.asp](https://www.w3schools.com/js/js_arrays.asp)

JavaScript functions are powerful tools used to encapsulate and reuse code. They allow you to define blocks of code that can be executed with a specific name and arguments. Here are some key things to know about them:

**1. Function definition:**

**JavaScript**

```jsx
function myFunction(name) {
  // Code to be executed
  console.log("Hello, " + name);
}

```

This defines a function named `myFunction` that takes a parameter named `name`. The code within the curly braces will be executed when the function is called.

**2. Calling a function:**

**JavaScript**

```jsx
myFunction("Bard"); // Output: "Hello, Bard"

```

This calls the `myFunction` with the value "Bard" passed as the `name` argument.

**3. Parameters and arguments:**

Functions can take multiple parameters, and each argument passed to the function call must correspond to the parameter order. You can also have default values for parameters.

**4. Return values:**

Functions can optionally return a value using the `return` keyword. This can be used to send data back from the function to the calling code.

**5. Function scope:**

Variables declared inside a function have local scope and are not accessible outside of the function.

**Here are some additional concepts related to JavaScript functions:**

- **Arrow functions:** A concise way to define anonymous functions.
- **Function expressions:** Functions can be assigned to variables or passed as arguments.
- **Closures:** Functions can access variables declared in their surrounding scope.
- **Callbacks:** Functions passed as arguments to other functions.

These are just a few basics of JavaScript functions. There are many more advanced features and techniques you can explore.

**Here are the key types of JavaScript functions, explained with visual aids:**

**1. Named Functions:**

- **Definition:** Functions declared with a name, allowing for multiple calls.
- **Syntax:**

**JavaScript**

```jsx
function functionName(parameters) {
  // Code to be executed
}

```

- **Example:**

**JavaScript**

```jsx
function greet(name) {
  console.log("Hello, " + name + "!");
}
greet("Alice"); // Output: Hello, Alice!

```

**2. Anonymous Functions:**

- **Definition:** Functions without a name, often used as arguments or for one-time use.
- **Syntax:**

**JavaScript**

```jsx
// As a variable:
const myFunction = function(parameters) {
  // Code to be executed
};

// As an argument:
setTimeout(function() {
  console.log("This runs after a delay");
}, 1000);

```

**3. Arrow Functions:**

- **Definition:** Concise syntax for functions, often used with callbacks and higher-order functions.
- **Syntax:**

**JavaScript**

```jsx
// Without parameters:
const myArrowFunction = () => {
  // Code to be executed
};

// With parameters:
const add = (x, y) => x + y;

```

**4. Generator Functions:**

- **Definition:** Functions that can be paused and resumed, used for iterators and efficient data management.
- **Syntax:**

**JavaScript**

```jsx
function* myGenerator() {
  yield 1;
  yield 2;
  yield 3;
}

```

**5. Async Functions:**

- **Definition:** Functions that handle asynchronous operations (like network requests) using `async` and `await` keywords.
- **Syntax:**

**JavaScript**

```jsx
async function fetchData() {
  const response = await fetch("https://api.example.com/data");
  const data = await response.json();
  console.log(data);
}

```

**6. Async Generator Functions:**

- **Definition:** Combine features of generator and async functions, for asynchronous iteration.
- **Syntax:**

**JavaScript**

```jsx
async function* myAsyncGenerator() {
  const response = await fetch("https://api.example.com/data");
  const data = await response.json();
  yield* data;
}

```

**Key Points:**

- Functions are reusable blocks of code.
- Choose the appropriate type based on use case.
- Consider readability, maintainability, and performance.

**Here's a comprehensive explanation of JavaScript objects:**

**What are JavaScript objects?**

- Objects are fundamental building blocks in JavaScript, used to represent complex data structures and real-world entities.
- They are collections of key-value pairs, where:
    - Keys are unique names (strings or symbols) that identify properties.
    - Values can be any data type, including numbers, strings, booleans, other objects, arrays, or even functions.

**Creating objects:**

1. **Object literal syntax:**
    
    **JavaScript**
    
    ```jsx
    const person = {
        firstName: "John",
        lastName: "Doe",
        age: 30,
        hobbies: ["coding", "reading"],
        greet: function() {
            console.log("Hello, my name is " + this.firstName);
        }
    };
    
    ```
    
2. **Constructor function:**
    
    **JavaScript**
    
    ```jsx
    function Person(firstName, lastName, age) {
        this.firstName = firstName;
        this.lastName = lastName;
        this.age = age;
    }
    
    const person2 = new Person("Jane", "Smith", 25);
    
    ```
    

**Accessing properties:**

- Use dot notation: `objectName.propertyName`
    
    **JavaScript**
    
    ```jsx
    console.log(person.firstName); // Output: John
    
    ```
    
- Use bracket notation: `objectName["propertyName"]` (useful for dynamic property names)
    
    **JavaScript**
    
    ```jsx
    const propertyName = "age";
    console.log(person[propertyName]); // Output: 30
    
    ```
    

**Modifying properties:**

- Assign new values to properties:
    
    **JavaScript**
    
    ```jsx
    person.age = 35;
    
    ```
    

**Adding new properties:**

- Simply assign a value to a new property name:
    
    **JavaScript**
    
    ```jsx
    person.city = "New York";
    
    ```
    

**Deleting properties:**

- Use the `delete` keyword:
    
    **JavaScript**
    
    ```jsx
    delete person.age;
    
    ```
    

**Key points:**

- Objects are mutable (their properties can be changed after creation).
- They are passed by reference (changes to an object affect all variables referencing it).
- The `this` keyword inside a method refers to the object itself.
- Objects can be nested to create complex data structures.
- They are essential for representing real-world data and organizing code in JavaScript applications.