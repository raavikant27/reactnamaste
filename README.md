# reactnamaste

/**episode
// this is syntex od reacte compnent
//**React component**//
// there are two type of commponent
//1- class based component -old way - nobody be use.
//2- functional component - new way of writing code
// react functional Component wht?
// just a normal javascript function. which return some javascript jsx.
// this is all it.
// jsx is react element , 
const HeadingComponent=React=()=>{
   return <h1>namste react functional component</h1>
}
// this  both function same,means function is returning true.
const fn = () => true;
// React element
const className = (
  <h1 className="head" tabIndex="5">
    namste ravikant
  </h1>
);

// react functional component
const HeadingComponent1 = () => (
  <div id="container">
    <h1 className="heading">Namaste react functional component</h1>
  </div>
);





   //**when we reden the heading elememnt so we write like this**/


   // this  both function same,means function is returning true.
const fn = () => true;
// React element
const className = (
  <h1 className="head" tabIndex="5">
    namste ravikant
  </h1>
);

// react functional component
const HeadingComponent1 = () => (
  <div id="container">
    <h1 className="heading">Namaste react functional component</h1>
  </div>
);


//**how will render  the compnent of**//

// React element
const className = (
  <h1 className="head" tabIndex="5">
    namste ravikant
  </h1>
);

// react functional component
const HeadingComponent1 = () => (
  <div id="container">
    <h1 className="heading">Namaste react functional component</h1>
  </div>
);
// we render the element

const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(<HeadingComponent1 />);
// we render 

///**component composition**////

 when two two componet compose to each other
 const Tittle = () => (
  <h1 className="head" tabIndex="5">
    namste ravikant
  </h1>
);

// react functional component
const HeadingComponent1 = () => (
  <div id="container">
    <Tittle />
    <h1 className="heading">Namaste react functional component</h1>
  </div>
);


const root = ReactDOM.createRoot(document.getElementById("root"));
// root. render convert everything in to html
root.render(<HeadingComponent1 />);
///**how we put elemnt in to js compnent using currely braches**////

const title = (
  <h1 className="head" tabIndex="5">
    ravikant
  </h1>
);
//u can anythiing javascipt express in currly barases
// it powerof jsx.
// writting javacript in to jsx very power full thing
// how we put react elment into the component.so we use tittle.

const Number = 1000;
// suppose data come from api
const data=api.getData();
const HeadingComponent1 = () => (
  <div id="container">
    {title}

    <h1>{Number}</h1>

    <h1 className="heading"> Namste reactcomponent</h1>
  </div>
);

//**how in compnent call to another react compnentt**//'
 using tittle  we call  component like {tittle()},<title><title>,</title>





 class works
 <h3> <a href="https://github.com/vaibhav1281/Namaste-React/blob/main/React-Day-2/Notes/README.md">Previous<< </a> </h3>

<P>Till now to run our project we use the command <code>npx parcel index.html</code></p>
<P><code>npx</code> means, we are executing <code>npm</code> package parcel, and we give the source file as <code>index.html</code></p>
<P>Now, we create script,that will build our project, instead of writing <code>npx parcel index.html</code> again and again, we use our custom script to run the project</p>
<P>We'll create this script inside the <code>package.josn</code> file</p>

```
 "scripts": {
    "start": "parcel index.html",
    "build": "parcel build index.html",
    "test": "jest"
  },
  ```
<p>Now to run our project,we'll use <code>npm run start</code> or <code>npm start</code> and for <b>Production build</b> we use <code>npm build</code></p>

<h2>Creating JSX Heading</h2>
<p>For single line of JSX code:</p>

```

const jsxHeading = <h1>Heading Using JSX</h1>

```
<p>For multiple lines of JSX code, we use Round Brackets</p>

```
const jsxHeading = (
    <h1 className="head">
        Heading Using JSX
    </h1>
)
```

<p>JSX is NOt HTML in JavaScript. HTML,React and JSX are thre different thing.</p>

<h3>Creating ReactElement using React</h3>

```
const heading = React.createElement(
  "h1",
  {id:"heading"},
  "Hello WOrld"
);
const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(heading);
```

<h3>Creating ReactElement using JSX</h3>

```
const jsxHeading = <h1 id="heading">Heading Using JSX</h1> 
const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(jsxHeading);
```

<h3>JSX Working</h3>

```

JSX => React.createElement => React Element (JavaScript Object) => (Renders)

```

<h3>React Componenet</h3>
<h4>There are two types of React Components</h4>
<ol>
  <li>Class Based Component</li>
  <li>Functional Component</li>
</ol>
<h3>Functional Component</h3>
<h4>This is how Functional Component are created</h4>
<p>When the code is single lined:</p>

```
const Heading = () => <h1>I am a functional component!</h1>
```
<p>When there multiple lines:</p>

```
Const Heading = () => {
  return (
    <div>
      <h2>I am a functional component!</h2>
    </div>
  )
}
```

<h3>How To Render React Functional Component</h3>

```
const Element1 = () => {
    return(
        <div className="title">

            <h1>Header 1 Using Functional component</h1>
            <h2>Header 2 Using Functional component</h2>
            <h3>Header 3 Using Functional component</h3>
            
        </div>
    );
};
const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(<Element1/>);

```

<h3>How We Can Render One Component Inside Another Component</h3>
<p>This Process is called <b>Component Composition</b></p>

```
const Element1 = () => {
    return(
        <div className="title">

            <h1>Header 1 Using Functional component</h1>
            <h2>Header 2 Using Functional component</h2>
            <h3>Header 3 Using Functional component</h3>
            
        </div>
    );
};

// Component Composition
const ComponentComposition = () => {
    return(
        <div>
            <h1>Here is the Component Composition</h1>

            <Element1/>
    
        </div>
    );
}
  
const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(<ComponentComposition/>);

```

<p></p>
<p></p>


 <h3 align="right"> <a href="https://github.com/vaibhav1281/Namaste-React/blob/main/React-Day-4/Notes/README.md">Next >></a> </h3>


 assignment
 <div align="right"> 
  
## [Assignment 04 >>]()
</div>

# Assignment 03
### Q.1. Create a Nested header Element using React.createElement(h1,h2,h3 inside a div with class "title")

### Code

```
/**
*   <div className="title">
*       <h1>Header 1</h1>
*       <h2>Header 2</h2>
*       <h3>Header 3</h3>
*   </div>
*/

import React from "react";
import  ReactDOM  from "react-dom";

const element = React.createElement(
    'div',
    { className: 'title' },
    React.createElement('h1', {}, 'Header 1'),
    React.createElement('h2', null, 'Header 2'),
    React.createElement('h3', {}, 'Header 3')
);

const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(element);

```

<h3>Output</h3>
<img alt="Code's Output" src="./OutputSS/Ans1.png"/>

### Q.1.1 Create the same element using JSX.

### Code

```
import React from "react";
import  ReactDOM  from "react-dom";

const jsxElement = (
    <div className="title">
        <h1>Header 1 Using JSX</h1>
        <h2>Header 2 Using JSX</h2>
        <h3>Header 3 Using JSX</h3>
    </div>
);

const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(jsxElement);

```

<h3>Output</h3>
<img alt="Code's Output" src="./OutputSS/Ans1.1.png"/>

### Q.1.2. Create a functional component of the same with JSX.

### Code

```

import React from "react";
import  ReactDOM  from "react-dom";

const Element1 = () => {
    return(
        <div className="title">

            <h1>Header 1 Using Functional component</h1>
            <h2>Header 2 Using Functional component</h2>
            <h3>Header 3 Using Functional component</h3>
            
        </div>
    );
};

const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(<Element1/>);

```

<h3>Output</h3>
<img alt="Code's Output" src="./OutputSS/Ans1.2.png"/>

### Q.1.3. Composition of Component (Add a component inside another)

### Code

```
import React from "react";
import  ReactDOM  from "react-dom";

/**
 *  <div className="title">
 *      <h1>
 *          <h2>
 *              <h3></h3>
 *          </h2>
 *      </h1>
 *  </div>
 */


const heading = React.createElement(
    "div",
    {className:"title"},
    React.createElement(
        "h1",
        {},
        React.createElement(
            "h2",
            {},
            React.createElement(
                "h3",
                {},
                "hello world"
            )
        )
    )
);


/**
*   <div className="title">
*       <h1></h1>
*       <h1></h1>
*       <h1></h1>
*   </div>
*/

const element = React.createElement(
    'div',
    { className: 'title' },
    React.createElement('h1', {}, 'Header 1'),
    React.createElement('h2', null, 'Header 2'),
    React.createElement('h3', {}, 'Header 3')
);

// Creating Same element using JSX

const jsxElement = (
    <div className="title">
        <h1>Header 1 Using JSX</h1>
        <h2>Header 2 Using JSX</h2>
        <h3>Header 3 Using JSX</h3>
    </div>
);

// Create a functional component of the same with JSX

const Element1 = () => {
    return(
        <div className="title">

            <h1>Header 1 Using Functional component</h1>
            <h2>Header 2 Using Functional component</h2>
            <h3>Header 3 Using Functional component</h3>
            
        </div>
    );
};

// Component Composition

const ComponentComposition = () => {
    return(
        <div>
            <h1>Here is the Component Composition</h1>
            {heading}
            <Element1/>
            {element}
            {jsxElement}
        </div>
    );
}
  
const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(<ComponentComposition/>);

```
<h3>Output</h3>
<img alt="Code's Output" src="./OutputSS/Ans1.3.png"/>

<h1> Q.2. Create a Header Component from scratch using Functional Components with JSX
    <ul>
        <li>Add a Logo on left</li>
        <li>Add a search bar in middle</li>
        <li>Add User icon on right Add CSS to make it look nice</li>
    </ul>
</h1>    

## Code 

```
import React from "react"
import ReactDOM from "react-dom/client"
import logo from "./images/logo.png"

const Heading = () => {
  return(
    <div>
      <div className="flex justify-between w-full h-[80px]">

        <img className="w-[80px] h-[80px] ml-10" src={logo} alt="logo" />
        
        <div className="">
          <ul className="flex flex-row space-x-10 text-lg mt-5 mr-10 font-semibold">
            <li><a href="#">Home</a></li>
            <li><a href="#aboutus">About Us</a></li>
            <li><a href="#contactus">Contact us</a></li>
          </ul>
        </div>


      </div>

      <div className="w-full h-10 flex items-center justify-center">
        <input
            type="text" 
            name="" 
            id="" 
            placeholder="Search..." 
            className="border border-gray-300 rounded py-2 px-4 w-[45%] mt-4"
            
        />
      </div>


    </div>
  )
}

const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(<Heading/>)
```

## Output
<img alt="Code's Output" src="./OutputSS/Ans2.png"/>


<div align="right"> 
  
## [Assignment 04 >>]()
</div>
 
   
