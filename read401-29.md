# How can we ensure that an effect hook runs only once?

![](https://res.cloudinary.com/practicaldev/image/fetch/s--g7tfK4Md--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/i/poh98tassqz2avu3j889.jpg)

**If we pass an empty array [] , it just renders the component only once like componentDidMount . Let's look at this example: import React, { useEffect, useState } from 'react'; function App() { const [count, setCount] = useState(0); useEffect(() => { console. log('Hello from useEffect!**

# Can useState() update more than one state variable at the same time?

**You could combine the loading state and data state into one state object and then you could do one setState call and there will only be one render. Note: Unlike the setState in class components, the setState returned from useState doesn't merge objects with existing state, it replaces the object entirely**

# Is useState() synchronous?
![](https://miro.medium.com/max/1400/0*t8rrmJTvGIZiAkhZ)

**useState and setState both are asynchronous. They do not update the state immediately but have queues that are used to update the state object. This is done to improve the performance of the rendering of React components. Even though they are asynchronous, the useState and setState functions do not return promises.**

| Term       |       Definition             |
| -----------|------------------------------|
|State Hook|A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We'll learn other Hooks later|
|Component Lifecycle|Components are created (mounted on the DOM), grow by updating, and then die (unmount on DOM). This is referred to as a component lifecycle. There are different lifecycle methods that React provides at different phases of a component's life.At present, we know what lifecycle methods are and why they are important.|