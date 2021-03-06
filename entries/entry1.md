# Entry 1: Introduction

## What is React.js?
React.js is a JavaScript Library for building user interfaces. A user interface is how a person interacts with a program. Therefore, in the MVC pattern this would be the view. Another JavaScript library that I am familiar with and have used before is p5js. The developers of this program are Facebook, Instagram, and other individuals. React.js was first released in March of 2013. The main reason why people use this is to provide speed and simplicity to large web-applications. This is due to the fact that React.js allows data to change over time without reloading the page. In other words, React will update and render data (UI/view) when it changes. This turns the JavaScript into a reactive language.

## How it works!

Dataset:

<img src="../images/entry1-data.png"/>
User Interface:

<img src="../images/entry1-view.png"/>

Let's say this is a web page. Here we have a dataset (Model) and a UI (View). We want the UI to reflect the dataset, and we also want it to update when a value changes. The issue with this is that the data is on the server and the UI is on a client computer (which is limited to HTML, CSS, JavaScript).

<img src="../images/mvc.png"/>

<img src="../images/DOM.png"/>

A Virtual DOM is the User Interface (UI) or the html page. ReactJS creates a virtual representation (in memory representation) of the DOM. And every time a change is made to the dataset (Model), it updates the entire Virtual DOM. Next, it performs a diff operation between the old virtual DOM (before it was updated) and the new virtual DOM that it just created. Then it determines which specific parts of the DOM have changed and updates ONLY those parts in the real dom. This process is very fast. Developers don't need to worry all they do is update the entire dom because ReactJS will handle what specifically gets rendered.

## Resources:
https://reactjs.org/

https://en.wikipedia.org/wiki/React_(JavaScript_library)

https://www.youtube.com/watch?v=JPT3bFIwJYA

https://www.youtube.com/watch?v=ycstRj2i66k