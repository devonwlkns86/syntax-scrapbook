# 🧠 Syntax-Scrapbook
/*

A personal, beginner-friendly reference for learning programming syntax!
This repository is my interactive "syntax scrapbook"—a place where 
I collect and organize small, easy-to-understand code examples 
for the languages 
I'm learning: HTML, CSS, JavaScript, React, and Python.

*/

My goal is to make syntax easier to remember by:

    Keeping code examples short and super clear

    Adding helpful comments and emojis to jog my memory

    Organizing examples by topic (like loops, functions, styling, etc.)

Whether you're also just starting out or just need a quick reminder, feel free to fork this and build your own scrapbook!

----------------------------------------------------------------------------------------------------------------------

 ✅ HTML - ## 🌐 HTML

🔤 Basic Structure

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My Page</title>
  </head>
  <body>
    <h1>Hello World</h1>
  </body>
</html>

🧠 Hint: Think of HTML like the skeleton of a website.

-------------------------------------------------------------------------------------------------------------------

🎨 CSS
body {
  background-color: #f0f0f0;
  font-family: sans-serif;
  color: #333;
}

🧠 Hint: CSS is like clothing for your HTML. It changes how things look.

------------------------------------------------------------------------------------------------------------------

📦 Flexbox (Beginner Version)

.container {
  display: flex;
  justify-content: center;
  align-items: center;
}

🧠 Hint: Flexbox helps you center and space stuff easily.

------------------------------------------------------------------------------------------------------------------

🟨 JavaScript (JS) - 🧮 Variables & Function

let name = "Devon";
function greet(user) {
  return "Hello, " + user + "!";
}
console.log(greet(name));


💡 JavaScript – Arrow Functions + Array Methods

// Transforming an array using .map and an arrow function
const numbers = [1, 2, 3, 4, 5];

// Double each number
const doubled = numbers.map(n => n * 2);

console.log(doubled); // [2, 4, 6, 8, 10]

✅ Highlights:

    Arrow function shorthand (n => n * 2)

    .map() for transforming arrays

    Clean and modern JS syntax


🔁 Loop

for (let i = 0; i < 5; i++) {
  console.log("Number: " + i);
}

🧠 Hint: Start, stop, step—i++ increases by 1.

--------------------------------------------------------------------------------------------------------------------

⚛️ React (JS Library) - 🧱 Basic Component

function Hello() {
  return <h1>Hello React!</h1>;
}

⚛️ React – useState Hook (State Management)

import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0); // Declare state variable

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>Click me!</button>
    </div>
  );
}

export default Counter;

✅ Highlights:

    useState hook for functional components

    setCount(count + 1) for updating state

    Event handling with onClick



🧠 Hint

  - Components always return JSX (HTML-like code)

  - Component names must start with a capital letter

-------------------------------------------------------------------------------------------------------------------

📦 Props Example

function Welcome(props) {
  return <h2>Welcome, {props.name}!</h2>;
}

🧠 Hint: Props are like function parameters.

-------------------------------------------------------------------------------------------------------------------

🐍 Python - 🐍 Print & Variable

name = "Devon"
print("Hello,", name)

🔁 Loop

for i in range(5):
    print("Number:", i)

✅ Function

def greet(user):
    return "Hi " + user


🐍 Python – List Comprehension with Condition

# List comprehension to filter and square even numbers
numbers = [1, 2, 3, 4, 5, 6]

squares_of_even = [n**2 for n in numbers if n % 2 == 0]

print(squares_of_even)  # [4, 16, 36]

✅ Highlights:

    Compact one-liner with for and if

    Readable and powerful filtering

    Common Python idiom!




🧠 Hint: Python uses colons : and indentation instead of {}

-------------------------------------------------------------------------------------------------------------------














