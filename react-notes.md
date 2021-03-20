# React Notes

`useState`

```jsx
import { useState, useEffect } from "react";

const [state, setState] = useState({});

setState(...);
/* set state does not have callback function because we used
   useState hook in a functional component.
   setState() is generally asynchronous function so if we desire
   a callback then we have to use it in useEffect hook.
*/

useEffect(() => {

}, [...]) 
/* the second argument is optional which allows us to pass in a
   variable or an array. If we pass in either of them then the
   function will fire when one of the variables change.
   This is a life saver.
*/

// Unknown Prop Warning
const { altMenuActive, ...rest } = props
// If using {...props} we can pass in unwanted props. So just pull
// what we don't want to pass in with {...props} and use the rest

```

TODO: Check if useEffect fires on component re-render or on-load when we put in the second argument because if it does not then it will be soooo helpful!



React mouse events: [https://reactjs.org/docs/events.html\#mouse-events](https://reactjs.org/docs/events.html#mouse-events)



