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
 
   
