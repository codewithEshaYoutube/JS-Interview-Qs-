# 🌟 Top 30 JavaScript Interview Questions for FAANG Companies 🌟

## 1. What is JavaScript?
- A high-level, interpreted programming language primarily used for web development.

---

## 2. Explain the difference between `var`, `let`, and `const`.
- **`var`**: Function-scoped or globally scoped, can be re-declared.
- **`let`**: Block-scoped, cannot be re-declared in the same block.
- **`const`**: Block-scoped, must be initialized at declaration, cannot be re-assigned.

---

## 3. What are closures in JavaScript?
- Functions that retain access to their lexical scope even when the function is executed outside that scope.

---

## 4. What is the event loop in JavaScript?
- A mechanism that handles asynchronous callbacks, allowing non-blocking I/O operations.

---

## 5. Explain the concept of hoisting.
- Variable and function declarations are moved to the top of their containing scope during compilation.

---

## 6. What are promises in JavaScript?
- Objects that represent the eventual completion (or failure) of an asynchronous operation and its resulting value.

---

## 7. How do you handle errors in JavaScript?
- Using `try...catch` statements, and promise `.catch()` for handling asynchronous errors.

---

## 8. What is the difference between synchronous and asynchronous code?
- **Synchronous**: Runs sequentially.
- **Asynchronous**: Allows other operations to run before completing a task.

---

## 9. Describe the `this` keyword in JavaScript.
- Refers to the object from which a function was called, context-dependent based on how a function is invoked.

---

## 10. What are arrow functions?
- Shorter syntax for writing functions, automatically binding `this` to the surrounding context.

---

## 11. What is the purpose of `bind()`, `call()`, and `apply()`?
- Methods to set the `this` context for functions:
  - **`bind()`**: Returns a new function with bound `this`.
  - **`call()`**: Invokes a function with a specified `this` value.
  - **`apply()`**: Similar to `call()`, but accepts an array of arguments.

---

## 12. Explain the concept of the prototype chain.
- Mechanism by which JavaScript objects inherit properties and methods from other objects through their prototype.

---

## 13. What are higher-order functions?
- Functions that take other functions as arguments or return them as output.

---

## 14. What is the difference between `==` and `===`?
- **`==`**: Abstract equality (coerces types).
- **`===`**: Strict equality (no type coercion).

---

## 15. Describe the `fetch` API.
- A modern interface for making HTTP requests, returning promises that resolve to the response of the request.

---

## 16. What is the significance of the `async` and `await` keywords?
- Used to work with promises in a more synchronous manner, making asynchronous code easier to read and write.

---

## 17. Explain destructuring assignment.
- A syntax that allows unpacking values from arrays or properties from objects into distinct variables.

---

## 18. What is the spread operator?
- A syntax (`...`) that expands an iterable into more elements, useful for array and object manipulation.

---

## 19. How does garbage collection work in JavaScript?
- Automatic memory management process that frees up memory by removing objects no longer in use.

---

## 20. What is a JavaScript module?
- A file or script that exports functions, objects, or variables, allowing code reuse and modularity.

---

## 21. Explain the concept of immutability.
- The state of an object cannot be modified after it is created, often used with libraries like Immutable.js.

---

## 22. What are template literals?
- String literals that allow embedded expressions, multi-line strings, and improved readability.

---

## 23. How do you optimize JavaScript performance?
- Techniques include minimizing DOM manipulation, using debouncing/throttling for events, and optimizing loops.

---

## 24. What are service workers?
- Scripts that run in the background, separate from web pages, enabling features like caching and background sync.

---

## 25. Explain the difference between `setTimeout` and `setInterval`.
- **`setTimeout`**: Executes a function once after a delay.
- **`setInterval`**: Repeatedly executes a function at specified intervals.

---

## 26. How do you retrieve data using a callback function in JavaScript?
### Example Code:
```html
<script>
// Simulated API call
function fetchUserData(callback) {
    setTimeout(() => {
        const userData = {
            name: "John Doe",
            age: 30,
            email: "john.doe@example.com"
        };
        // Call the callback function with the retrieved data
        callback(userData);
    }, 1000); // Simulates a 1-second delay
}

// Callback function to process user data
function processUserData(data) {
    console.log("User Data Retrieved:");
    console.log(`Name: ${data.name}`);
    console.log(`Age: ${data.age}`);
    console.log(`Email: ${data.email}`);
}

// Retrieve user data and process it
fetchUserData(processUserData);
</script>
