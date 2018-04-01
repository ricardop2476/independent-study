# Entry 2: Using Resources

## ReactJS Course
In order to keep on learning about ReactJS I decided to find resources online that would help me learn more about this concept. A Google search helped me find out that Codecademy has a course dedicated just to ReactJS. This is a website that I am very familiar with, and I have used this site to learn about various other languages. When I read the course description I learned that one essential component of ReactJS is JSX. I remember seeing this term in the official website of ReactJS. A quick search at their website (https://reactjs.org/) I found out the following: 👇

> React components implement a `render()` method that takes input data and returns what to display. This example uses an XML-like syntax called JSX. Input data that is passed into the component can be accessed by `render()` via `this.props`. JSX is optional and not required to use React.

* With JSX
```
class HelloMessage extends React.Component {
  render() {
    return (
      <div>
        Hello {this.props.name}
      </div>
    );
  }
}

ReactDOM.render(
  <HelloMessage name="Taylor" />,
  mountNode
);
```
* Without JSX
```
class HelloMessage extends React.Component {
  render() {
    return React.createElement(
      "div",
      null,
      "Hello ",
      this.props.name
    );
  }
}

ReactDOM.render(React.createElement(HelloMessage, { name: "Taylor" }), mountNode);
```
Both of these output "Hello Taylor"

From a visual standpoint I can already tell that JSX format makes code easier to read and also is more organized. I saw if the Codecademy course had a JSX section by checking the syllabus, and I found out that they did.

## What I Learned About JSX
JSX is a syntax extension for JavaScript. It was written to be used with React. JSX code is similar HTML. JSX is not valid JavaScript because web browsers can't read it. If a JavaScript file contains JSX code, before the file reaches a web browser, a JSX compiler will translate any JSX into regular JavaScript.

One of the most basic JSX elements would be code similar to HTML.
`<h1>Hello world</h1>`
The difference is that you would find this in a JavaScript file and not a HTML file.

I also learned that, JSX elements are treated as JavaScript expressions. They can go anywhere that JavaScript expressions can go. This means that a JSX element can be saved in a variable, passed to a function, stored in an object or array. I did a Google search for 'javascript expressions' and got a similar result. I learned that there are two types of expressions: those that assign a value to a variable, and those that simply have a value.

## Learning From Mistakes
When creating a JSX `<article></article>` element and saving it in a variable named `myArticle` I did this initially:

`myArticle = <article></article>`

I got an error, and found out that in JavaScript files lines of code should start with `const` and end with `;`. Correct code:

`const myArticle = <article></article>;`

## Takeaways
In my learning process I learned that before diving into a tutorial or online guide it is okay to reinforce your learning with knowledge that you do not understand. If key words pop up in summaries prior to completing a tutorial google them. Even a general idea will help you, because in the tutorial you will get a more defined idea. When I learn anything, I understand it more if I do it more than once. Even during your learning process (not just initially) google terms that you do not understand because if you don't, you will be more confused in the future.
## Resources:
https://www.codecademy.com/learn/react-101

https://reactjs.org/