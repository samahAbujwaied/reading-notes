# How granular should your reducers be?

![](https://res.cloudinary.com/practicaldev/image/fetch/s--nQ4oHNpH--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/sx9yndandw37b3sgg3r9.png)

**Both the Redux core library and most of the Redux documentation are unopinionated. There are many ways to use Redux, and much of the time there is no single "right" way to do things.**

**However, time and experience have shown that for some topics, certain approaches work better than others. In addition, many developers have asked us to provide official guidance to reduce decision fatigue.***
# Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

**As with state, serializable actions enable several of Redux's defining features, such as time travel debugging, and recording and replaying actions. Using something like a Symbol for the type value or using instanceof checks for actions themselves would break that. Strings are serializable and easily self-descriptive, and so are a better choice. Note that it is okay to use Symbols, Promises, or other non-serializable values in an action if the action is intended for use by middleware. Actions only need to be serializable by the time they actually reach the store and are passed to the reducers.**

# Name a strategy for preventing the above
![](https://www.china-briefing.com/news/wp-content/uploads/2018/09/CB-Outsourcing.jpg)

| Term       |       Definition             |
| -----------|------------------------------|
|store|A store. js plugin is a function that returns an object that gets added to the store. If any of the plugin functions overrides existing functions, the plugin function can still call the original function using the first argument (super_fn).|
|combined reducers|Combine reducers takes a hash of reducers and returns a reducer. The resulting reducer represents an object of the same shape as the hash. So, a call like this: combineReducers({ name: nameReducer}) Would produce a state object that might look something like this: { name: 'Joe Shmo' }|