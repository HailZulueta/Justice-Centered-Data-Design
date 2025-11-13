# Functions

A function is a reusable set of statements that embody the following qualities:

1. **Accept Inputs**: Uses 1 or more incoming data parameters delivered from another place in the code, where the function is called.
2. **Performs a Task**: Within the scope of the function, the inputs can be used to whatever you define to produce new values.
3. **Returns an Output**: After the task is performed on the inputs, you can `return` a desired value back to where the function was called in your code.

In order to use a function, you must define it somewhere in the scope where you wish to call it.

```javascript
// Define my cool function
const suggestDogName = (incomingString) => {
  let suggestion = `You should name your dog **${incomingString}**!`
  return suggestion
}

let dogName = "Luna"
// Call suggestDogName and provide parameter value to send as input
let dogNameSuggestion = suggestDogName(dogName)

console.log(dogNameSuggestion)
// Logs String of "You should name your dog **Luna**!"
```

## Parameters, i.e., Inputs

- Inputs to functions are called *parameters*.
- Parameters are defined by an ordered list of variables written within the paranthesis: `(param1, param2, param3, ...)`.
- Parameters will have the value of whatever is passed to the function in the order.
- Parameters become variables to use only inside the scope of the function's body demarcated by curly braces `{...}`.
- Functions do not need to include parameters.

## return Statements

Functions return (pass back) values to where it was called by using the `return` keyword.

- The `return` statement ends a function's execution immediately, since it passes the value back to where the function was originally called in the scope of the javascript file.
- A common mistake: Forgetting to use a `return` statement, so the default returned value will become `undefined`.
- Another common mistake: Using the `return` statement in the wrong scope of your function's code. Sometimes we write nested scopes, so it can become easy to write our `return` statement in the wrong scope. For example, perhaps you write a `return` statement too soon within the scope of a `for..loop`, rather than after the `for...loop` is complete.
