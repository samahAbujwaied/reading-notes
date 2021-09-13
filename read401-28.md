# Why do we not need more .html pages in a multi-page React app? 
![](https://i.imgur.com/thYo8iK.png)

**create-react-app provides a great starting point to start a new react app fully configured with webpack, live reloading, etc. But, sadly, it doesn't provide a way to provide different index files with a different set of entry points.**

# If we wanted a component to show up on every page, where would we put it and why? 
 
 **Inside a <Route />, so we can access it**

# What does routing do with the components that were rendered when a new route is requested ?

- renders the appropriate user interface when the current location matches the route’s path. 
-  The component prop defines the React element that will be returned by the Route when the path is matched. This React element is created from the provided component using React.createElement.

# What does props.children contain?

![](https://soshace.com/wp-content/uploads/2019/08/React-Children-Cheat-Sheet.png)

**props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a component. This component contains an <img> that is receiving some props and then it is displaying {props.**

# How do useState() and this.setState() differ?
- The setState function is used to handle the state object in a React class component. 
-  setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won't touch the rest. The useState's updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.

| Term       |       Definition             |
| -----------|------------------------------|
|State Hook|A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We'll learn other Hooks later|
|Mounting and Un-Mounting|Mounting a file system attaches that file system to a directory (mount point) and makes it available to the system.The root ( / ) file system is always mounted. Any other file system can be connected or disconnected from the root ( / ) file system|