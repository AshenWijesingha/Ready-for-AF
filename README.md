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
- In this example, we have a functional component called ```Greeting``` that returns a JSX element ```<h1>Hello World!</h1>```, which represents the greeting message. Then, in the ```App``` component, we render the ```Greeting``` component, encapsulated in a ```div``` element.

- To run this app, you'll need to set up a React development environment, including installing Node.js and creating a new React project using a tool like Create React App. Once the project is set up, replace the content of the ```App.js``` file with the code provided and start the development server.

- When you open the app in your browser, you should see the greeting "Hello World!" displayed on the screen.

<hr>

- Create a "NavBar" component that displays a navigation menu.
1. Start by creating a new React component called "NavBar".
2. Inside the "NavBar" component, return a JSX element that displays a navigation menu. This can be a simple unordered list with a few links to different pages or sections of your app.
3. Render the "NavBar" component in your main app component.

```jsx
import React from 'react';

// Step 1: Create a new React component called "NavBar"
const NavBar = () => {
  // Step 2: Return a JSX element that displays a navigation menu
  return (
    <nav>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/about">About</a></li>
        <li><a href="/contact">Contact</a></li>
      </ul>
    </nav>
  );
};

// Step 3: Render the "NavBar" component in your main app component
const App = () => {
  return (
    <div>
      <NavBar />
      {/* Your other app content goes here */}
    </div>
  );
};

export default App;
```
- In this example, we have a functional component called ```NavBar``` that returns a JSX element representing a navigation menu. The navigation menu is structured as an unordered list (```<ul>```) with several list items (```<li>```), each containing an anchor tag (```<a>```) representing a link to a different page or section of the app. You can modify the ```href``` attribute of the anchor tags to point to the appropriate URLs in your application.

- In the ```App``` component, we render the ```NavBar``` component, followed by your other app content. The ```NavBar``` component will be displayed at the top of the app, and you can place the rest of your app's content below it.

- Remember to set up your React development environment and replace the content of the ```App.js``` file with the code provided.

  ### OR

  #### NavBar.js:

  ```jsx
  import React from 'react';

    const NavBar = () => {
      return (
        <nav>
          <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/about">About</a></li>
            <li><a href="/contact">Contact</a></li>
          </ul>
        </nav>
      );
    };

export default NavBar;
  ```

#### Home.js:

```jsx
import React from 'react';

const Home = () => {
  return <h1>Welcome to the Home Page!</h1>;
};

export default Home;
```

#### About.js:

```jsx
import React from 'react';

const About = () => {
  return <h1>About Us</h1>;
};

export default About;
```

#### Contact.js:

```jsx
import React from 'react';

const Contact = () => {
  return <h1>Contact Us</h1>;
};

export default Contact;
```

#### App.js:

```jsx
import React from 'react';
import NavBar from './NavBar';
import Home from './Home';
import About from './About';
import Contact from './Contact';

const App = () => {
  return (
    <div>
      <NavBar />
      <Home />
      {/* Your other app content goes here */}
      <About />
      <Contact />
    </div>
  );
};

export default App;
```

- In this updated example, each page component (```Home```, ```About```, ```Contact```) is created in separate files and imported into the ```App.js``` file. The ```NavBar``` component is also created in a separate file and imported.

- Ensure that all the component files are in the same directory as the ```App.js``` file or adjust the import paths accordingly if they are in different directories.

- By organizing your code into separate files, it becomes easier to manage and maintain your React application.

<hr>

