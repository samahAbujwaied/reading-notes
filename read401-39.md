# What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application? 

![](http://semantic-portal.net/images/react-native-database-selection/IMAGE2-610x300.png)

**The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.**

# When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
![](https://redux.js.org/assets/images/ReduxAsyncDataFlowDiagram-d97ff38a0f4da0f327163170ccc13e80.gif)

**The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.**

| Term       |       Definition             |
| -----------|------------------------------|
|middleware|Middleware functions are functions that have access to the request object ( req ), the response object ( res ), and the next middleware function in the application's request-response cycle. The next middleware function is commonly denoted by a variable named next |
|thunk|A thunk is just a function which delays the evaluation of the value. The thunk function doesn't take any arguments and gives the value whenever you invoke the thunk.|