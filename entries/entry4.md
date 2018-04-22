# Entry 4: React Components

## What is a React Component?
A component is a small, reusable chunk of code that is responsible for one job. That job is often to render some HTML. Every component must come from a component class. Everything in React is a component which makes it easy to reuse components frequently. So if there is a webpage, a button might be a component, or a div with several items in it. The code below is responsible for creating and rendering a React Component. 

``` javascript
import React from 'react';
import ReactDOM from 'react-dom';

class MyComponentClass extends React.Component {
  render() {
    return <h1>Hello world</h1>;
  }
};

ReactDOM.render(
  <MyComponentClass />,
  document.getElementById('app')
);
```

<strong>[Line 1] `import React from 'react';`</strong> <br>
We created a new variable named `React`, and its value is a particular, imported JavaScript object, which contains methods that we need in order to use React. We need these in order for React to work, and some of the methods that we obtain are, `React.createElement()` and `React.Component`. The object is called the React library.

<strong>[Line 2] `import ReactDOM from 'react-dom';`</strong> <br>
The methods imported from `'react-dom'` are meant for interacting with the DOM. In other words, `import ReactDOM` from `'react-dom'` creates another JavaScript object. This object contains methods that help React interact with the DOM, such as `ReactDOM.render()`.

<strong>[Line 4] `class MyComponentClass extends React.Component`</strong> <br>
A component class is like a factory that creates components. If you have a component class, then you can use that class to produce as many components as you want. To make a component class, you use a base class from the React library: `React.Component`. `React.Component` is a JavaScript class. To create your own component class, you must <strong>subclass</strong> `React.Component`. You can do this by using the syntax `class YourComponentNameGoesHere extends React.Component {}`. By subclassing `React.Component`, you create a new component class. This is not a component! A component class is more like a factory that produces components. When you start making components, each one will come from a component class.

<strong>[Lines 4-7] The body of the component class
``` javascript
class MyComponentClass extends React.Component {
  render() {
    return <h1>Hello world</h1>;
  }
};
```
</strong>
Like all JavaScript classes, this one needs a body. The body will act as a set of instructions, explaining to your component class how it should build a React component. <br>
The render function: There is only one property that you have to include in your instructions: a render method. A *render method* is a property whose name is render, and whose value is a function. The term "render method" can refer to the entire property, or to just the function part. A render method must contain a return statement. Usually, this return statement returns a JSX expression. A render method must contain a return statement. Usually, this return statement returns a JSX expression. In other words, it holds component views. Component’s render method will return JSX which then it uses to create a real HTML output which will be rendered in the browser. It only runs when your component State or Props updates.

<strong>[Line 11] `<MyComponentClass />,` </strong> <br>
This line of code will call its render method, which will return the JSX element `<h1>Hello world</h1>`. `ReactDOM.render()` will then take that resulting JSX element, and add it to the virtual DOM. This will make `"Hello world"` appear on the screen. We can use this component anywhere inside our react application by writing this line of code. (To make a React component, we write a JSX element. Instead of naming the JSX element something like h1 or div like before, we give it the same name as a component class.)

## Sources:
https://codeburst.io/react-components-explained-96718311f20b
