how to pass props in router.....
import React from 'react';
import { Route } from 'react-router-dom';

// Define your component that you want to render
function Contact(props) {
  return (
    <div>
      <h1>Contact Page</h1>
      <p>Name: {props.name}</p>
      <p>Email: {props.email}</p>
    </div>
  );
}

// In your route configuration, use the render function to pass props
<Route
  path="/contact"
  element={<Contact name="John Doe" email="john@example.com" />}
/>
diffrence btwn compo and render method....
render method dont update when we call again and again it only call when some thing is change.........
but it component it will every time update and give new value to u.....
just think about painting example....
if we are not using any props.....then use component otherwise props...
.....
The useParams hook returns an object of key/value pairs of the dynamic params from the current URL that were matched by the <Route path>. Child routes inherit all params from their parent routes.....
use params hooks is used to show dynamically any data in component....

by using uselocation....we can findout the current path....
 const location=useLocation();....

 
 note...
 this repo cover some of basic concept of....
 react-router
 search effect using useState
 simple navbar using router
 some hooks like params, useLocation, useHistory
 props in router....
 