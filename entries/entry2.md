# Entry 2: Using Resources

## ReactJS Course
In order to keep on learning about ReactJS I decided to find resources online that would help me learn more about this concept. A Google search helped me find out that Codecademy has a course dedicated just to ReactJS. This is a website that I am very familiar with, and I have used this site to learn about various other languages. When I read the course description I learned that one essential compontent of ReactJS is JSX. I remember seeing this term in the offical website of ReactJS. A quick search at thier website (https://reactjs.org/) I found out the following: 👇

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
## Resources:
https://www.codecademy.com/learn/react-101

https://reactjs.org/