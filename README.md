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

## ⚛️ React Development Notes

### 🟢 Running the Local Dev Server

Each time you want to run your React app locally, follow these steps:

```bash
cd /path/to/project
npm run dev


This starts the development server (usually at http://localhost:5173)

Your app will reload automatically as you make changes.

⚠️ Don’t close the terminal! If you close it, the server shuts down.


USE THIS >>>>> to restart the APP again if need be >>>>> npm run dev


Optional: Open your project folder in VS Code and run the above command inside the built-in terminal.

>>>>>>>>     

-----------------------------------------------------------------------------------------------------------------------

>>>    RRRRRRR)))
   >>>   EEEEEEEE)))
      >>>    AAAAAAA)))
         >>>    CCCCCCC)))
            >>>     TTTTTTT)))


# ⚛️ React Basics – Syntax Scrapbook

## 📘 What is React?

React is a **JavaScript library** for building **dynamic user interfaces** using reusable components.  
It combines **JavaScript logic** with **HTML-like syntax** (called **JSX**).

---

## 💡 Core Concepts

### 🧩 Components
React apps are built from **components** – reusable pieces of UI.

```jsx
function MovieCard(props) {
  return <div>{props.title}</div>;
}

Use them like HTML tags:

<MovieCard title="Inception" />

🧠 useState – Track Dynamic Data (State)

import { useState } from 'react';

function Example() {
  const [count, setCount] = useState(0);

  return (
    <button onClick={() => setCount(count + 1)}>
      Clicked {count} times
    </button>
  );
}

🔄 useEffect – Handle Side Effects (like API calls)

import { useEffect } from 'react';

useEffect(() => {
  // runs when component mounts
  fetchMovies();
}, []);

🧭 Routing – React Router

npm install react-router-dom

Example routes:

import { BrowserRouter, Route, Routes } from 'react-router-dom';

<BrowserRouter>
  <Routes>
    <Route path="/" element={<Home />} />
    <Route path="/movie/:id" element={<MovieDetails />} />
  </Routes>
</BrowserRouter>

🔁 Rendering Lists

movies.map(movie => (
  <MovieCard key={movie.id} title={movie.title} />
));

🚦 Conditional Rendering

{isLoading ? <LoadingSpinner /> : <MovieList />}

🎨 Styling Options

You can style your components using:

    CSS Modules

    Tailwind CSS

    Styled Components

    Regular CSS

Example with Tailwind:

<div className="bg-black text-white p-4 rounded-lg">Movie Card</div>

🔌 Fetching API Data

Example with TMDB:

const API_KEY = "your_key";
const URL = `https://api.themoviedb.org/3/movie/popular?api_key=${API_KEY}`;

fetch(URL)
  .then(res => res.json())
  .then(data => setMovies(data.results));

✅ Summary Table
Feature	Description
JSX	HTML-like syntax inside JS
Components	Reusable UI building blocks
useState	Tracks dynamic app data
useEffect	Handles side effects like API calls
react-router-dom	Adds multiple routes/pages
.map()	Loop through lists and render items
Conditional render	Show/hide UI based on logic
Styling	Use Tailwind, CSS Modules, etc.
API Integration	Use fetch/axios to load real data















