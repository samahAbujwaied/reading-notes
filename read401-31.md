# Describe use cases useState() vs useReducer() ? 
![](https://res.cloudinary.com/practicaldev/image/fetch/s--_bonmxpu--/c_imagga_scale,f_auto,fl_progressive,h_500,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/heahvzlsz9a1eh23mjw9.png)

**useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks**

# Why do custom hooks need the use prefix?
![](https://miro.medium.com/max/1400/1*sft5y71BAgqxBrKHJcmYkg.png)

**We can decide what it takes as arguments, and what, if anything, it should return. In other words, it's just like a normal function. Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it**

# What do custom hooks usually do?
![](https://miro.medium.com/max/2756/1*X3yhCiSjWvR7I93Q4gop5Q.png)

**Custom hooks are a handy way to encapsulate hook-related logic that can be re-used across components when using component composition isn't really something that will help, make sense, or just "look" semantically right.**

# Using any list of custom hooks, research and name one that you think will be useful in your applications 
**Custom React Hooks allow us to extract component logic into reusable functions. Custom Hooks look very much like normal helper functions, except they can maintain component state and perform effects. So if you find yourself using a lot of these Hooks, you might as well import the package.**

# Describe how a hook that fetches API data might work 
![](https://rapidapi.com/blog/wp-content/uploads/2020/04/final_app-300x132.png)

**Put the fetchData function above in the useEffect hook and call it, like so: useEffect(() => { const url = "https://api.adviceslip.com/advice"; const fetchData = async () => { try { const response = await fetch(url); const json = await response. json(); console. log(json); } catch (error) { console.**

| Term       |       Definition             |
| -----------|------------------------------|
|Reducer|A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change.Redux relies heavily on reducer functions that take the previous state and an action in order to execute the next state.|