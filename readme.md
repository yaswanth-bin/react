React is a open source library not framework.<br>
It focuses more on UI.<br>
It is created and maintained by Facebook.<br>
React is component based architecture.<br>
Components are useful in reuse of code<br>
React was first developed by Jordan Walke(2011)fax.js<br>
In 2013 React.js became open source<br>
## How to setup project
npm create vite@latest<br>
npm run dev<br>
JSX stands for javascript xml<br>
JSX element = a JavaScript representation of UI that looks like HTML<br>
without jsx:
const p = React.createElement("p",null,"hello");
with jsx:
const p = <p>Hello</p>
<br>
ReactDOM.createRoot(document.getElementById("root")).render(p);
## component:
->A component is a piece of reusable code in UI<br>
->A function that returns jsx element<br>
ex:
```
function Greeting() {
  return <h1>Hello, world!</h1>;
}
ReactDOM.createRoot(document.getElementById("root")).render(<Greeting/>);
```
## props:
props (short for properties) are used to pass data from one component to another.<br>
ex:
```
function Welcome(props) {
  return <h1>Hello {props.name}</h1>;
}
<Welcome name="Yaswanth" />
```
you should not change props inside a function (or anywhere in a component).
## export and import :
export default componentName(Test.jsx file)<br>
import componentName(any name if it is default) from './Test';
## class based component:
```
import React from "react";

class Welcome extends React.Component {
  render() {
    return <h1>Hello {this.props.name}</h1>;
  }
}

export default Welcome;
```
```
import Welcome from "./Welcome";

function App() {
  return <Welcome name="Yaswanth" />;
}
```
