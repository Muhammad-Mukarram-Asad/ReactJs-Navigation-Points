# ReactJs-Navigation-Points
React Naviagtion is the central feature of a web application by which a user can anviagte from one page to another based on his request
or actions.
From a basic HTML website to a complex application built using frameworks like Reactjs, whenever you want to use URL in your application or react native apps, react navigation comes into play.
React Router is a library built on top of React for enabling programmatic React navigation by handling routes in a web application. The react navigation library allows the UI to be in sync with the browser URL by conditionally displaying components.
Moreover, it also allows browser functionalities like the back button and page refresh. Using React Router is considered to be the standard routing solution in React and is made use by popular social media mobile apps like Facebook and Instagram. 
# Installing react-router-dom
To use React Router in your react app or react native apps, all you need to do is install the dependency.
yarn add react-router-dom
OR
npm install react-router-dom --save   
Note: The current version is React Router v6.
Configuring routes
After installation, now it is time to configure the routes. The steps are as below:

# Step 1:
Go to ./src/App.js file inside your project.
# Step 2:
Import the following components of react-router-dom inside this js file.

# BrowserRouter         
# Route 
# Routes
import {
  BrowserRouter,
  Routes, //replaces "Switch" used till v5
  Route,
} from "react-router-dom";
Also, import all the components that need to be returned within each route.

# Step 3:
Wrap the content of the App component within the <BrowserRouter>.
function App() {
  return (
    <div className="App">
      <BrowserRouter>
        ....
      </BrowserRouter>
    </div>
  );
}
# Step 4:
Now within the children content, wrap the part of the UI that needs to conditionally render a certain component based configuration on the URL inside <Routes>.

Within <Routes>, mention each case of <Route> by defining the following attributes:

path – for the URL
element – for the component that needs to be rendered for that URL
