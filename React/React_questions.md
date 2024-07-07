# 1. React Basic

## 1. What is React.js?

React.js is a front-end and open-source library for building complex and reusable components. The components can run in website and moblie applications.

Important Feature

1. Server-Side Render
2. Virtual DOM
3. Undirection data binding
4. JSX

## 2. What is React Hooks?

Before React 16.8, only class components were used for state management and lifecycle method, function components were only used for stateless components. After React 16.8, React has hooks and allows function components to manage state and lifecycle, which make coding easier, cleaner and more flexibility.

## 3. What is useState()

useState is one of hooks in React. It will return a tuple, the first param is the current state, the second param is a function which allow us to update the state. It helps us control the variable state. For example, I want to develop a counting website. Every time I click the button, the count will increase. I can use setState return [count, setCount], count is the value, setCount is the function that helps us increase.