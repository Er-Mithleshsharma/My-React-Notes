# React Notes

## Introduction

React is a JavaScript library for building user interfaces. It allows developers to create reusable UI components and efficiently update the UI when data changes.

## Key Concepts

### Components

- Components are the building blocks of a React application.
- They encapsulate UI elements and logic, making the code modular and easier to maintain.
- React components can be either functional or class-based.

### JSX (JavaScript XML)

- JSX is a syntax extension for JavaScript that allows you to write HTML-like code within JavaScript.
- It makes React code more readable and expressive.
- JSX elements are transpiled into regular JavaScript function calls.

### Props

- Props (short for properties) are used to pass data from parent to child components.
- They are read-only and help make components reusable by allowing them to accept different sets of data.

### State

- State is an object that represents the internal state of a component.
- It allows components to manage their own data and re-render when the state changes.
- State should be treated as immutable to ensure predictable component behavior.

### Lifecycle Methods

- Lifecycle methods are special methods that are invoked at various stages of a component's lifecycle.
- They allow you to perform actions such as initializing state, fetching data, and updating the DOM.
- Common lifecycle methods include `componentDidMount`, `componentDidUpdate`, and `componentWillUnmount`.

### Hooks

- Hooks are functions that allow functional components to use state and other React features.
- They enable you to reuse stateful logic without writing class components.
- Commonly used hooks include `useState`, `useEffect`, and `useContext`.

## Example

```jsx
import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={() => setCount(count + 1)}>Increment</button>
    </div>
  );
}

export default Counter;
