# Why choose Redux instead of the Context API for global state?
![](https://miro.medium.com/max/1200/0*9PpL94nNCBcomuLf.png)

**context API is easy to is use as it has a short learning curve. It requires less code, and because there's no need of extra libraries, bundle sizes are reduced. Redux on the other hand requires adding more libraries to the application bundle. The syntax is complex and extensive creating unnecessary work and complexity**

# What is the purpose of a reducer?

**In Redux, a reducer is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action**

# What does an action contain?
![](https://media.geeksforgeeks.org/wp-content/uploads/20191016141017/redux.png)\

**Actions are the only source of information for the store as per Redux official documentation. It carries a payload of information from your application to store. As discussed earlier, actions are plain JavaScript object that must have a type attribute to indicate the type of action performed.**

| Term       |       Definition             |
| -----------|------------------------------|
|Immutable state|In object-oriented and functional programming, an immutable object (unchangeable object) is an object whose state cannot be modified after it is created. This is in contrast to a mutable object (changeable object), which can be modified after it is created|
|Time travel in redux|Time travel is the ability to move back and forth among the previous states of an application and view the results in real time. With Redux, given a specific state and a specific action, the next state of the application is always exactly the same.|
|action creator|An action creator is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function.|
|reducer| reducer is a very simple idea and it's something that will be easy for you to grasp because, in a nutshell, it's just a simple JS function. A reducer is a function which takes two arguments — the current state and an action — and returns based on both arguments a new state|
|dispatch|dispatch is a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change. With React Redux, your components never access the store directly - connect does it for you.|