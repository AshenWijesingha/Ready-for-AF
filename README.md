# Ready-for-AF
Ready for Application Frameworks Module Final Examination.

# React

- Create a simple "Hello World" app that displays a greeting message to the user.
1. Start by creating a new React component called "Greeting".
2. Inside the "Greeting" component, return a JSX element that displays a greeting message to the user, such as "Hello World!".
3. Render the "Greeting" component in your main app component

```jsx
import React from 'react';

// Step 1: Create a new React component called "Greeting"
const Greeting = () => {
  // Step 2: Return a JSX element that displays a greeting message
  return <h1>Hello World!</h1>;
};

// Step 3: Render the "Greeting" component in your main app component
const App = () => {
  return (
    <div>
      <Greeting />
    </div>
  );
};

export default App;
```
In this example, we have a functional component called ```Greeting``` that returns a JSX element ```<h1>Hello World!</h1>```, which represents the greeting message. Then, in the ```App``` component, we render the ```Greeting``` component, encapsulated in a ```div``` element.

To run this app, you'll need to set up a React development environment, including installing Node.js and creating a new React project using a tool like Create React App. Once the project is set up, replace the content of the ```App.js``` file with the code provided and start the development server.

When you open the app in your browser, you should see the greeting "Hello World!" displayed on the screen.
