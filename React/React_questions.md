1. # React Basic

1. ## What is React.js?

React.js is a front-end and open-source library for building complex and reusable components. The components can run in website and moblie applications.

Important Feature

1. Server-Side Render
2. Virtual DOM
3. Undirection data binding
4. JSX

1. ## What is React Hooks?

Before React 16.8, only class components were used for state management and lifecycle method, function components were only used for stateless components. After React 16.8, React has hooks and allows function components to manage state and lifecycle, which make coding easier, cleaner and more flexibility.

There are two rules.

**Only function components can use hooks.**

React Hooks **must be called only at the top level**. It is not allowed to call them inside the nested functions, loops, or conditions.

1. ## What is useState()

useState is one of hooks in React. It will return a tuple, the first param is the current state, the second param is a function which allow us to update the state. It helps us control the variable state. For example, I want to develop a counting website. Every time I click the button, the count will increase. I can use setState return [count, setCount], count is the value, setCount is the function that helps us increase.

1. ## What is useEffect()

useEffect is a hooks for processing side effects. We can use effect to do something after rendering and state changed. 

useEffect() accepts two params. **useEffect(callback,[dependencies])**

Callback function will execute immediately when page renders first time and dependencies changed every times. When dependencies are empty array. The callback will only excute once the first time.

1. ## What is JSX.

JavaScript XML. It allows us write HTML code inside the JS code without using function

1. ## What are keys in React?

We can use keys for list rendering by Arrays.map. Give every item a unique key. Keys should be from API data.

1. ## What is virtual DOM

Every real DOM has copied virtual DOM, which has the same properties. And virtual DOM has two virtual DOM, one is prev virtual DOM, one is updated virtual DOM. And React finds the diff between two virtual DOM, and rendering the changed real DOM in the website, instead of rendering all DOM. ( Because most JavaScript frameworks update the entire DOM even when a small part of the DOM changes.)

Two virtual DOM data structures: tree, only same level tag will compare 

![img](https://f6wrt0e6n4.feishu.cn/space/api/box/stream/download/asynccode/?code=YTJlNjY3MjFhOWRkYzJmODM1ZmZlM2Y1YWEwMjgxM2RfZHpNUjZadGJRcm54bUVQcHJZM3BKWFJ1ME5GR2xpek1fVG9rZW46RkczWWI3WWdobzh0TWF4dnpSbGN4eVg2bnJkXzE3MjA0MDM4Nzg6MTcyMDQwNzQ3OF9WNA)

Algorithm: DFS  

Time complexity: O(N) 

1. ## What is Props

Props is input for a react component. It can be single-value or object. The props is used to deliver data from one components to another components.

Using inside render() in components by this.props.reactProp.

Props is read only. But we can modify its value by creating a new state

Sample:

```JavaScript
<Element reactProps = '1'/>

function Element(props){
    const [element, setElement] = useState(props.reactProps)
}
```

1. ## What is the difference between props and state.

![img](https://f6wrt0e6n4.feishu.cn/space/api/box/stream/download/asynccode/?code=MjkzODdkMTE2Nzc5NzlhNzQ3ZGRiY2ViYTY2YWYyYzBfQ3I5MEpidmlGRFU3TVFvSkZveEQwajdjMGhZVnVPMlNfVG9rZW46UmwyZWJKOXFab3pnall4MDF2MWNJallBbldmXzE3MjA0MDM4Nzg6MTcyMDQwNzQ3OF9WNA)

1. ## What is the difference between hooks and classes.

![img](https://f6wrt0e6n4.feishu.cn/space/api/box/stream/download/asynccode/?code=OTg5OTFhMGYyZjVkMjJiNzhjZjhhNzNlYmRlMDgzYmZfUzhLNjZSVGlYV3BoNnMwRjhVWnF6NFVGTUJFVThLZjNfVG9rZW46WTY0RmJlbnBab1o1d014a3daWmNRMHNmblNBXzE3MjA0MDM4Nzg6MTcyMDQwNzQ3OF9WNA)

1. ## What is callback function?

Callback function is usually as a param that passed to another function. When an event happens, the callback function will be called.

As a props, from parents components to children components.

As an event, such as onClick = {callback function}

Handle the async, such as fetch the data.

As a useEffect callback function.